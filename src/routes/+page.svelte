<main>
<div class="grid-6" style="padding-block:2%;">
       
    <div class="card">
     <img src="https://images.unsplash.com/photo-1534528741775-53994a69daeb?ixlib=rb-4.0.3&ixid=MnwxMjA3fDB8MHxwaG90by1wYWdlfHx8fGVufDB8fHx8&auto=format&fit=crop&w=464&q=80" class="imagen-principal" alt="Portrait">
     
    </div>
    
         
            
    <div class="card">
     
      <h3 class="nombre">Hi , I'm <span>Pablo</span> </h3>
     <h4 class="based">I'm a developer based in Chile</h4>
          
     <p style="line-height: 1.8rem;"> 
    I have a passion for technology and am always looking to learn and improve my skills.
    My skillset includes HTML, CSS, JavaScript, and various frameworks and libraries such as React and Svelte. In my free time, I enjoy making music and exploring new ways to express myself creatively.
    </p>
     <a href="/readmore"><button class="boton">Read More</button></a>

     </div>


 </div>
</main>
<br>
<br>
<br>
<!-- aca termina el card main-->





 <!-- aca empieza el grid portfolio-->


 
 <div class="grid-6" style="background-color:#efb229 ; padding-inline: 2%;">
    <center><h2 class="portfolio">PROJECTS</h2></center>     
    <div class="card">
    
     <img src="https://images.unsplash.com/photo-1499951360447-b19be8fe80f5?ixlib=rb-4.0.3&ixid=MnwxMjA3fDB8MHxwaG90by1wYWdlfHx8fGVufDB8fHx8&auto=format&fit=crop&w=870&q=80" class="card-imagen-horizontal" alt="imagen of lucy Mckenzie">

     <a href="https://magazine-puce.vercel.app/"><button class="card-boton">LIVE</button></a>
     <a href="https://magazine-puce.vercel.app/"><button class="card-boton">CODE</button></a>

     <h4 class="card-portfolio-text-big">Magazine</h4><br>
     
     <p class="card-portfolio-text">McKenzie collaborates with other creatives regularly. Through her collaborations, she challenges the notion of authorship by pointing to the strength of collective actions. </p>

    

    </div>
           
            
    <div class="card">
     <img src="https://images.unsplash.com/photo-1587440871875-191322ee64b0?ixlib=rb-4.0.3&ixid=MnwxMjA3fDB8MHxwaG90by1wYWdlfHx8fGVufDB8fHx8&auto=format&fit=crop&w=871&q=80" class="card-imagen-horizontal" alt="imagen of emily speed" >

     <h4 class="card-portfolio-text-big">Emily Speed</h4><br>
          
     <p class="card-portfolio-text">Experience a new film installation by North West based artist Emily Speed. The film is inspired by Edwin Abbott’s 1884 novella Flatland, a satire of Victorian society. </p>
     </div>

   

      <div class="card">
       <img src="https://images.unsplash.com/photo-1522542550221-31fd19575a2d?ixlib=rb-4.0.3&ixid=MnwxMjA3fDB8MHxzZWFyY2h8MTh8fHdlYiUyMGRlc2lnbnxlbnwwfHwwfHw%3D&auto=format&fit=crop&w=500&q=60" class="card-imagen-horizontal" alt="imagen of emily speed" >

       <h4 class="card-portfolio-text-big">VALIS</h4><br>
            
       <p class="card-portfolio-text">And I love the kind of ongoing love affair, aesthetically and politically, between Black Americans and Puerto Ricans. There’s been so much synergy, especially in the Bronx, in East Harlem, Lower East Side, and parts of Brooklyn.</p>
       </div>


       <div class="card">
         <img src="https://images.unsplash.com/photo-1517134191118-9d595e4c8c2b?ixlib=rb-4.0.3&ixid=MnwxMjA3fDB8MHxwaG90by1wYWdlfHx8fGVufDB8fHx8&auto=format&fit=crop&w=870&q=80" class="card-imagen-horizontal" alt="imagen of lucy Mckenzie">
         <h4 class="card-portfolio-text-big">Love Your Work</h4><br>
         
         <p class="card-portfolio-text">Can architecture and design write scenarios for the next generation of work? What will it take to anticipate and formulate work environments and experiences that are productive, humane, and ecologically responsible? </p>
        </div>


        <div class="card">
         <img src="https://images.unsplash.com/photo-1497091071254-cc9b2ba7c48a?ixlib=rb-4.0.3&ixid=MnwxMjA3fDB8MHxwaG90by1wYWdlfHx8fGVufDB8fHx8&auto=format&fit=crop&w=874&q=80" class="card-imagen-horizontal" alt="imagen of lucy Mckenzie">
         <h4 class="card-portfolio-text-big">Harvard Design</h4><br>
         
         <p class="card-portfolio-text">Contemporary public space projects should address both the digital and the physical layer of a place. The two are becoming increasingly interconnected and dependent on each other. </p>
        </div>

 </div>



 

 <style>
   .nombre{
    font-size: 2rem;
   }
   .based{
    font-size: 1.4rem;
    margin-top: -1.6rem;
   }

    .grid-6{
    margin-top: 1rem;
    display: grid;
    grid-template-columns:repeat(auto-fit, minmax(21rem, 1fr)) ;
    padding: 5%;
    gap: 3rem;
}

.imagen-principal{
    width: 100%;
    aspect-ratio: 1/1;
    object-fit: cover;
    box-shadow:
      0 1px 1px hsl(0deg 0% 0% / 0.075),
      0 2px 2px hsl(0deg 0% 0% / 0.075),
      0 4px 4px hsl(0deg 0% 0% / 0.075),
      0 8px 8px hsl(0deg 0% 0% / 0.075),
      0 16px 16px hsl(0deg 0% 0% / 0.075);
    border-radius: 3px;
}

.card-imagen-horizontal{
    width: 100%;
    aspect-ratio: 1.5/1.1;
    object-fit: cover;
   
}

.card > h3 > span {
    border-bottom:3px solid #efb229;
    border-radius: 2px;
}

.boton {
  background-color:#efb229;
  border: none;
  color: blanchedalmond;
  padding: 15px 32px;
  text-align: center;
  text-decoration: none;
  display: inline-block;
  font-size: 18px;
  border-radius: 3px;
  transition: all 0.5s;
  
}

.boton:hover{
    color: black;
    cursor: pointer;
    transform: scale(1.05);
}


.portfolio{
    margin-top: 25%;
    align-items: center;
    justify-content: center;
    font-size:3rem ; 
    letter-spacing:1.7rem;
    color: wheat;
    font-weight: 900;
}
@media (max-width: 600px) {
    .portfolio{
        font-size: 1.8rem;
    }
}



.card-portfolio-text-big{
    text-align: center;
    font-size: 1.3rem;
    margin-top: 0rem;
    
}

.card-portfolio-text{
    margin-top: -2.5rem;
    text-align: center;
    
}

.card-boton {
  background-color:#efb229;
  border: none;
  margin-right: 2rem;
  margin-block: 0.6rem;
  color:wheat;
  padding: 8px 23px;
  text-align: center;
  text-decoration: none;
  font-size: 18px;
  border-radius: 3px;
  border: 1.2px solid black;
  transition: all 0.5s; 
  
  box-shadow:
      0 1px 1px hsl(0deg 0% 0% / 0.075),
      0 2px 2px hsl(0deg 0% 0% / 0.075);
      
}

.card-boton:hover{
    color: black;
    cursor: pointer;
    transform: scale(1.05);
}



 </style>

