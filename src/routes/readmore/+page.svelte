<script>
	import { _ } from 'svelte-i18n';
</script>

<div class="readme">
	<h3>TECH STACK</h3>
	<div class="container-badges">
		<div class="container-badges-group">
			<div class="container-badges-card">
				<img
					src="https://www.svgrepo.com/show/120930/html.svg"
					alt="html5 svg icon"
					class="icon-badge"
				/>
				<br />
				<br />
				<p>{$_('html')}</p>
			</div>

			<div class="container-badges-card">
				<img
					src="https://www.svgrepo.com/show/185568/file-css.svg"
					alt="css3 svg icon"
					class="icon-badge"
				/>
				<br />
				<br />
				<p>{$_('css')}</p>
			</div>
		</div>

		<div class="container-badges-group">
			<div class="container-badges-card">
				<img
					src="https://cdn.worldvectorlogo.com/logos/logo-javascript.svg"
					alt="javascript svg icon"
					class="icon-badge"
				/>
				<br />
				<br />
				<p>{$_('javascript')}</p>
			</div>

			<div class="container-badges-card">
				<img
					src="https://www.svgrepo.com/show/374304/git.svg"
					alt="git svg icon"
					class="icon-badge"
				/>
				<br />
				<br />
				<p>{$_('git')}</p>
			</div>
		</div>

		<div class="container-badges-group">
			<div class="container-badges-card">
				<img
					src="https://www.svgrepo.com/show/354259/react.svg"
					alt="react svg icon"
					class="icon-badge"
				/>
				<br />
				<br />
				<p>{$_('react')}</p>
			</div>

			<div class="container-badges-card">
				<img
					src="https://www.svgrepo.com/show/374109/svelte.svg"
					alt="svelte svg icon"
					class="icon-badge"
				/>
				<br />
				<br />
				<p>{$_('svelte')}</p>
			</div>
		</div>

		<div class="container-badges-group">
			<div class="container-badges-card">
				<img
					src="https://www.svgrepo.com/show/355038/golang.svg"
					alt="golang mascot svg icon"
					class="icon-badge"
				/>
				<br />
				<br />
				<p>{$_('python')}</p>
			</div>
			<div class="container-badges-card">
				<img
					src="https://www.svgrepo.com/show/373446/astro.svg"
					alt="astro svg icon"
					class="icon-badge"
				/>
				<br />
				<br />
				<p>{$_('astro')}</p>
			</div>
		</div>
	</div>

	<br />
	<br />
	<br />
	<!-- BIO -->
	<h3>{$_('moreAboutMe')} ✋</h3>
	<p>
		{$_('j1')}
	</p>

	<p>
		{$_('j3')}
	</p>

	<p>
		{$_('f1')}
	</p>
	<section>
		<h3>{$_('courses')}</h3>
		<ul>
			<li>CS50 Web Programming With Python and Javascript</li>
			<li>Introduction to Typography</li>
			<li>Web Development With React</li>
			<li>Introduction to Software Engineering</li>
			<li>Ideas From the History of Graphic Design</li>
			<li>Write JavaScript For The Web</li>
		</ul>
	</section>

	<br />
	<br />
	<br />
</div>

<style>
	.readme {
		align-items: center;
		margin-inline: 18rem;
		text-align: left;
		max-width: 1120px;
	}
	h3 {
		font-size: 2rem;
		border-bottom: 3px solid #efb229;
	}

	p {
		font-size: 1.1rem;
		margin-top: -1.3rem;
		margin-bottom: 2.5rem;
	}

	.icon-badge {
		width: 100px;
		align-items: center;
	}
	.container-badges {
		display: flex;
		flex-direction: column;
		margin: auto;
		gap: 20px;
		margin-inline: 4rem;
	}
	.container-badges-group {
		display: flex;
		flex-direction: row;
		justify-content: space-between;
		gap: 2rem;
		text-align: center;
	}
	.container-badges-card {
		background-color: #f1e1c3;
		/* border: 2px solid #A19D8F;  */
		border-radius: 10px;
		padding-inline: 1rem;
		padding-top: 1rem;
		display: flex;
		flex-direction: column;
		align-items: center;
		width: 40rem;
		min-height: 300px;
		box-shadow: 0 1px 1px hsl(0deg 0% 0% / 0.075), 0 2px 2px hsl(0deg 0% 0% / 0.075),
			0 4px 4px hsl(0deg 0% 0% / 0.075);
	}

	/* CURSOS LISTA */
	ul {
		margin: 0;
		padding: 0;
		font-size: 1.1rem;
		list-style: none;
	}
	li {
		padding: 0.5rem 1rem;
		margin: 0.5rem;
		border-bottom: #efb229 1px solid;
		border-radius: 8px;
		transition: all 1s;
	}
	li:hover {
		background-color: #efb229;
	}
	/* FIN CURSOS LISTA */

	/* MEDIA QUERIES */
	@media (max-width: 1120px) {
		.container-badges-group {
			flex-direction: column;
		}
		.container-badges-card {
			width: 30rem;
			margin-inline: auto;
		}
		.readme {
			margin-inline: 8rem;
		}
	}
	@media (max-width: 900px) {
		.container-badges-card {
			width: 25rem;
		}
	}
	@media (max-width: 800px) {
		.readme {
			margin-inline: 0.5rem;
		}
		.container-badges-group {
			margin-inline: -3.5rem;
		}

		.container-badges-card {
			width: 18rem;
		}
	}
</style>
