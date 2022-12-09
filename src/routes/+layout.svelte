
<nav class="barra-navegacion">
    <a class="nombre" href="/"><h3 >pablozuta</h3></a>
    <div class="icons">
       <a href="https://www.moma.org/"> <img src="https://www.svgrepo.com/show/353136/github.svg" alt="coding icon"></a>
        <a href="https://victoryjournal.com/"><img src="https://www.svgrepo.com/show/137277/twitter.svg" alt="web design icon"></a>
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
}
.nombre:hover{
   cursor: pointer;
    color: bisque;
}


</style>