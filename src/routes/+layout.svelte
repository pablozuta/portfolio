<script>
    import './../i18n'
    import { _ , addMessages, init } from 'svelte-i18n'
   
   
     init({ initialLocale:"es"});
   
     function cambioLenguajeEspaĆ±ol() {
       init({initialLocale:"es"})
       }
     function cambioLenguajeIngles() {
       init({initialLocale:"en"})
       }
     
     
</script>

<nav class="barra-navegacion">
    <a class="nombre" href="/"><h3 >pablozuta</h3></a>
    
    
    
    <div class="icons">
        <button on:click={cambioLenguajeEspaĆ±ol} class="boton">ES</button>
      <button on:click={cambioLenguajeIngles} class="boton">EN</button>
      <!--icono link a github-->
       <a href="https://github.com/pablozuta"> <img src="https://www.svgrepo.com/show/353136/github.svg" alt="github icon"></a>

    <!--icono link a twitter-->   
        <a href="https://twitter.com/theCodeOfPablo"><img src="https://www.svgrepo.com/show/137277/twitter.svg" alt="twitter icon"></a>
    </div>
</nav>

<slot></slot>

<style>
.barra-navegacion{
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

.nombre{
    letter-spacing: 0.1rem;
    list-style: none;
    text-decoration: none;
    color: black;
    font-size: 1.2rem;
}
.nombre:hover{
   cursor: pointer;
    color: bisque;
}
.boton{
    background-color: transparent;
    padding-inline: 1rem;
    padding-block: 0.3rem;
    margin-right: 0.1rem;
    font-size: 1rem;
    font-weight: 600;
    
    border: none;
}
.boton:hover{
   cursor: pointer;
   border-bottom: 1px solid #555;
   
}


</style>