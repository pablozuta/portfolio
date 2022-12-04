<nav class="barra-navegacion">
    <a class="nombre" href="/"><h3 >pablozuta</h3></a>
    <div class="icons">
        <img src="https://www.svgrepo.com/show/353136/github.svg" alt="coding icon">
        <img src="https://www.svgrepo.com/show/137277/twitter.svg" alt="web design icon">
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
    margin-right: 2rem;
    justify-content: center;
}

.icons > img {
    width: 22px;
    margin-left: 2rem;
    
}

.nombre{
    letter-spacing: 0.1rem;
    list-style: none;
    text-decoration: none;
    color: black;
}
.nombre:hover{
   cursor: pointer;
    color: bisque;
}


</style>