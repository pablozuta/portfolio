<script>
	// se importa el archivo con los textos de idiomas ingles y español
	import './../i18n';

	// se importan las utilidades que se usaran de la libreria svelte-i18n
	import { _, addMessages, init } from 'svelte-i18n';

	// se configura el lenguaje default (español)
	init({ initialLocale: 'es' });

	function cambioLenguajeEspañol() {
		init({ initialLocale: 'es' });
	}
	function cambioLenguajeIngles() {
		init({ initialLocale: 'en' });
	}
</script>

<header>
	<nav class="barra-navegacion">
		<a class="nombre" href="/"><h3>Portfolio</h3></a>

		<div class="icons">
			<button on:click={cambioLenguajeEspañol} class="boton">ES</button>
			<button on:click={cambioLenguajeIngles} class="boton">EN</button>
			<!--icono link a github-->
			<a href="https://github.com/pablozuta">
				<img src="https://www.svgrepo.com/show/353136/github.svg" alt="icono github svg" /></a
			>
		</div>
	</nav>
</header>

<slot />

<footer>
	<p>{$_('footerText')} <a class="link-footer" href="https://kit.svelte.dev/"> SvelteKit</a></p>
	<p>Copyright© 2023</p>
</footer>

<style>
	.barra-navegacion {
		background-color: #efb229;
		position: sticky;
		height: 3rem;
		top: 0;
		display: flex;
		align-items: center;
		justify-content: space-between;
		padding-inline: 1rem;
	}

	.icons {
		display: flex;
		flex-direction: row;
		justify-content: center;
	}

	.icons > a > img {
		width: 22px;
		margin-left: 2rem;
	}

	.nombre {
		letter-spacing: 0.1rem;
		list-style: none;
		text-decoration: none;
		color: black;
		font-size: 1.2rem;
	}
	.nombre:hover {
		cursor: pointer;
		color: bisque;
	}
	.boton {
		background-color: transparent;
		padding-inline: 1rem;
		padding-block: 0.3rem;
		margin-right: 0.1rem;
		font-size: 1rem;
		font-weight: 600;

		border: none;
	}
	.boton:hover {
		cursor: pointer;
		border-bottom: 1px solid #555;
	}

	/* FOOTER */
	footer {
		display: flex;
		font-size: 1.1rem;
		justify-content: center;
		align-items: center;
		background-color: #efb229;
		letter-spacing: 0.2rem;
		gap: 0.3rem;
	}
	.link-footer {
		text-decoration: none;
		color: bisque;
	}
	.link-footer:hover {
		color: black;
	}
	@media (max-width: 900px) {
		footer{
			flex-direction: column;
			letter-spacing: 0rem;
		}
	}
</style>
