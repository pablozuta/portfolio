<script>
	import { _ } from 'svelte-i18n';

	import { createClient } from '@supabase/supabase-js';
	import * as yup from 'yup';

	const supabaseUrl = import.meta.env.VITE_SUPABASE_URL;
	const supabaseKey = import.meta.env.VITE_SUPABASE_KEY;
	const supabase = createClient(supabaseUrl, supabaseKey);

	const validationSchema = yup.object({
		email: yup.string().email().required(),
		message: yup.string().required()
	});

	let email = '';
	let message = '';

	async function submitForm() {
		const { error } = await supabase.from('messages').insert({ email, message });

		if (error) {
			console.error(error);
		} else {
			email = '';
			message = '';
		}
		alert('mensaje enviado exitosamente.');
	}

	function handleSubmit(event) {
		event.preventDefault();

		validationSchema
			.validate({ email, message })
			.then(() => {
				submitForm();
			})
			.catch((error) => {
				console.error(error);
			});
	}
</script>

<section>
	<div class="form">
		<form on:submit={handleSubmit} class="card-form">
			<div>
				<input
					type="email"
					id="email"
					name="email"
					bind:value={email}
					placeholder="your email"
					class="email-input"
				/>
			</div>
			<div>
				<textarea id="message" name="message" bind:value={message} class="message-input" />
			</div>
			<center> <p>{$_('message')}</p></center>
			<button type="submit" class="button-form">Submit</button>
		</form>
	</div>
	<div class="image">
		<img
			src="https://res.cloudinary.com/ddkgbgwvp/image/upload/v1680732023/undraw_programming_re_kg9v_ttobxn.svg"
			alt="ilustration coding"
		/>
	</div>
</section>

<style>
	section {
		display: flex;
		margin-block: 2rem;
		justify-content: space-evenly;
		align-items: center;
		max-width: 1200px;
	}

	img {
		margin-inline: auto;
		display: grid;
		max-width: 24rem;
		aspect-ratio: 1/1;
		object-fit: contain;

		justify-items: center;
	}

	.form {
		display: flex;
		flex-direction: column;
		border: 2px solid #c4a660;
		border-radius: 10px;
		justify-content: space-between;
		align-items: center;
		flex-wrap: wrap;
		width: 32rem;
		height: 22rem;
		margin: 0 auto;
		padding: 1rem;
	}

	.email-input {
		display: flex;
		margin-inline: auto;
		align-self: center;
		justify-content: space-between;
		width: 24rem;
		margin-bottom: 16px;
		padding: 12px;
		border: none;
		border-radius: 4px;
		font-size: 16px;
		line-height: 1.5;
		background-color: #fff;
	}

	.message-input {
		background-color: #f1f1f1;
		border: none;
		border-radius: 4px;
		font-size: 16px;
		line-height: 1.3;
		width: 25.3rem;
		height: 10rem;
		resize: none;
	}

	.button-form {
		display: block;
		margin: 0.5rem auto;
		padding: 12px 24px;
		border: none;
		border-radius: 4px;
		font-size: 16px;
		font-weight: bold;
		text-transform: uppercase;
		color: #fff;
		background-color: #ddbc6e;
		cursor: pointer;
	}

	.button-form:hover {
		background-color: #c4a660;
	}

	.button-form:focus {
		outline: none;
		box-shadow: 0 0 0 2px rgba(47, 52, 58, 0.5);
	}
	@media (max-width: 900px) {
		section {
			flex-direction: column;
		}
		img {
			display: none;
		}
		.form {
			width: 22rem;
		}
		.message-input {
			margin-inline: 1rem;
			width: 18rem;
			height: 10rem;
		}
		.email-input {
			width: 17rem;
		}
	}
</style>
