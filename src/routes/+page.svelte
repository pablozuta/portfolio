<script>
	import { _ } from 'svelte-i18n';
</script>

<main>
	<div class="grid-6" style="padding-block:2%;">
		<div class="card">
			<img
				src="https://images.unsplash.com/photo-1534528741775-53994a69daeb?ixlib=rb-4.0.3&ixid=MnwxMjA3fDB8MHxwaG90by1wYWdlfHx8fGVufDB8fHx8&auto=format&fit=crop&w=464&q=80"
				class="imagen-principal"
				alt="Portrait"
			/>
		</div>

		<div class="card">
			<h3 class="nombre">{$_('greet')}<span>Pablo</span></h3>
			<h4 class="based">{$_('dev')}</h4>

			<p style="line-height: 1.8rem;">
				{$_('have')} <strong>{$_('have2')}</strong>
				{$_('have3')}
			</p>
			<a href="/readmore"><button class="boton">{$_('readMore')}</button></a>
		</div>
	</div>
</main>
<br />
<br />
<br />
<!-- aca termina el card main-->

<!-- aca empieza el grid portfolio-->

<div class="grid-6" style="background-color:#efb229 ; padding-inline: 2%;">
	<div class="container-project-text">
		<h2 class="portfolio">PROJECTS</h2>
		<h2 class="portfolio">PROJECTS</h2>
		<h2 class="portfolio">PROJECTS</h2>
		<h2 class="portfolio">PROJECTS</h2>
		<h2 class="portfolio">PROJECTS</h2>
	</div>

	<!--inicio card social media app-->
	<div class="card">
		<img
			src="https://images.unsplash.com/photo-1516251193007-45ef944ab0c6?ixlib=rb-4.0.3&ixid=MnwxMjA3fDB8MHxwaG90by1wYWdlfHx8fGVufDB8fHx8&auto=format&fit=crop&w=870&q=80"
			class="card-imagen-horizontal"
			alt="imagen social media"
		/>
		<div class="container-botones-card">
			<!--botones con links a webpage y repositorio-->
			<a href="https://social-eight-alpha.vercel.app/">
				<button class="card-boton">LIVE</button>
			</a>

			<!--termino botones con links a webpage y repositorio-->
		</div>

		<br />

		<p class="card-portfolio-text">
			{$_('social')}
		</p>
	</div>
	<!--termino card social media app-->


	<!--inicio card art magazine-->
	<div class="card">
		<img
			src="https://taiwanhappygo.com/wp-content/uploads/2021/07/%E5%92%96%E5%95%A1%E6%9B%B8.jpg"
			class="card-imagen-horizontal"
			alt="art magazine"
		/>
  
		<div class="container-botones-card">
			<!--botones con links a webpage y repositorio-->
			<a href="https://magazine-puce.vercel.app/">
				<button class="card-boton">LIVE</button>
			</a>
  
			<!--termino botones con links a webpage y repositorio-->
		</div>
		<br />
		
		<p class="card-portfolio-text">
			{$_('art')}
		</p>
	</div>
	<!--termino card art magazine-->
  
  

	


	<!--inicio card tipografia-->
	<div class="card">
		<img
			src="https://images.unsplash.com/photo-1581080247486-57989c1f14ab?ixlib=rb-4.0.3&ixid=MnwxMjA3fDB8MHxwaG90by1wYWdlfHx8fGVufDB8fHx8&auto=format&fit=crop&w=869&q=80"
			class="card-imagen-horizontal"
			alt="imagen de libro tipografia"
		/>
		<div class="container-botones-card">
			<!--botones con links a webpage y repositorio-->
			<a href="https://typography-svelte.vercel.app/">
				<button class="card-boton">LIVE</button>
			</a>

			<!--termino botones con links a webpage y repositorio-->
		</div>
		<br />

		<p class="card-portfolio-text">
			{$_('typo')}
		</p>
	</div>
	<!--termino card tipografia-->

  <!--inicio card go by example-->
  <div class="card">
    <img
      src="https://nextbridge.com/wp-content/uploads/2021/06/Go-Programming-Language-%E2%80%93-Making-a-Mark.jpg"
      class="card-imagen-horizontal"
      alt="imagen escritorio con notebook y taza de cafe"
    />
    <div class="container-botones-card">
      <!--botones con links a webpage y repositorio-->
      <a href="https://go-con-ejemplos.vercel.app/">
        <button class="card-boton">LIVE</button>
      </a>

      <!--termino botones con links a webpage y repositorio-->
    </div>
    <br />
    
    <p class="card-portfolio-text">
      {$_('blog')}
    </p>
  </div>
  <!-- termino card go by example-->



  <!--inicio card crypto market-->
	<div class="card">
		<img
			src="https://images.unsplash.com/photo-1634704784915-aacf363b021f?ixlib=rb-4.0.3&ixid=MnwxMjA3fDB8MHxwaG90by1wYWdlfHx8fGVufDB8fHx8&auto=format&fit=crop&w=870&q=80"
			class="card-imagen-horizontal"
			alt="imagen de bitcoin"
		/>
		<div class="container-botones-card">
			<!--botones con links a webpage y repositorio-->
			<a href="https://coin-market-chi.vercel.app/">
				<button class="card-boton">LIVE</button>
			</a>

			<!--termino botones con links a webpage y repositorio-->
		</div>
		<br />

		<p class="card-portfolio-text">
			{$_('crypto')}
		</p>
	</div>
	<!--termino card crypto market-->

</div>

<style>
	.nombre {
		font-size: 2rem;
	}
	.based {
		font-size: 1.4rem;
		margin-top: -1.6rem;
	}

	.grid-6 {
		margin-top: 1rem;
		display: grid;
		grid-template-columns: repeat(auto-fit, minmax(21rem, 1fr));
		padding: 5%;
		gap: 3rem;
	}

	.imagen-principal {
		margin-inline: auto;
		display: grid;
		width: 85%;
		aspect-ratio: 1/1;
		object-fit: cover;
		box-shadow: 0 1px 1px hsl(0deg 0% 0% / 0.075), 0 2px 2px hsl(0deg 0% 0% / 0.075),
			0 4px 4px hsl(0deg 0% 0% / 0.075), 0 8px 8px hsl(0deg 0% 0% / 0.075),
			0 16px 16px hsl(0deg 0% 0% / 0.075);
		border-radius: 3px;
		justify-items: center;
		
	}

	.card-imagen-horizontal {
		width: 100%;
		aspect-ratio: 1.5/1.1;
		object-fit: cover;
	}

	.card > h3 > span {
		border-bottom: 3px solid #efb229;
		border-radius: 2px;
	}

	.container-botones-card {
		display: flex;
		margin-bottom: 1rem;
		justify-content: flex-start;
		margin-top: -0.4rem;
	}

	.boton {
		background-color: #efb229;
		border: none;
		color: black;
		padding: 15px 32px;
		text-align: center;
		text-decoration: none;
		display: inline-block;
		font-size: 18px;
		border-radius: 3px;
		transition: all 0.5s;
	}

	.boton:hover {
		color: blanchedalmond;
		cursor: pointer;
		transform: scale(1.05);
	}

	.container-project-text {
		padding: 0;
		margin: 0;
		margin-top: -0.5rem;
		margin-right: 20%;
		flex-wrap: wrap;
		justify-content: flex-start;
		display: flex;
		flex-direction: column;
	}

	.portfolio {
		margin-block: -0.1rem;
		font-size: 2.9rem;
		letter-spacing: 1.5rem;
		color: #fc5d41;
		font-weight: 900;
		line-height: 4.1rem;
	}
	@media (max-width: 600px) {
		.portfolio {
			font-size: 1.9rem;
			letter-spacing: 1.3rem;
			margin: auto;
			margin-left: 1.9rem;
		}
	}

	.card-portfolio-text {
		margin-top: -2.5rem;
		text-align: left;
	}

	.card-boton {
		background-color: #efb229;
		border: none;
		margin-right: 2rem;
		margin-block: 0.6rem;
		color: #121212;
		padding: 8px 19px;
		text-align: left;
		text-decoration: none;
		font-size: 1.1rem;
		border-radius: 3px;
		border: 1.8px solid black;
		transition: all 0.5s;
		letter-spacing: 0.2rem;
	}

	.card-boton:hover {
		color: blanchedalmond;
		cursor: pointer;
		transform: scale(1.05);
	}
</style>
