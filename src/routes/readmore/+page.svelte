<script>
  import { _ } from 'svelte-i18n'
</script>

<div class="readme">
  <h3>{$_('journey')}</h3>
  <p>
    {$_('j1')}
  </p>
  <p>
   {$_('j2')}
  </p>
 
  <p>
    {$_('j3')}
  </p>

  <h3>{$_('future')}</h3>
  <p>
   {$_('f1')}
  </p>
 

  <h3>TECH STACK</h3>
  <div class="container-badges">
    <p class="badges">
      
      <a href="https://www.w3.org/html/" target="_blank" rel="noreferrer">
        <img
          src="https://www.svgrepo.com/show/120930/html.svg"
          alt="html5"
          class="icon-badge"
        /> </a>
       
        
       
       
    

      <a href="https://www.w3schools.com/css/" target="_blank" rel="noreferrer">
        <img
          src="https://www.svgrepo.com/show/185568/file-css.svg"
          alt="css3"
          class="icon-badge"
        /> 
      </a>

      <a
        href="https://developer.mozilla.org/en-US/docs/Web/JavaScript"
        target="_blank"
        rel="noreferrer"
      >
        <img
          src="https://cdn.worldvectorlogo.com/logos/logo-javascript.svg"
          alt="javascript"
          class="icon-badge"
        />
      </a>

      <a href="https://git-scm.com/" target="_blank" rel="noreferrer">
        <img
          src="https://www.svgrepo.com/show/374304/git.svg"
          alt="git"
          class="icon-badge"
        />
      </a>

      <a href="https://reactjs.org/" target="_blank" rel="noreferrer">
        <img
          src="https://www.svgrepo.com/show/354259/react.svg"
          alt="react"
          class="icon-badge"
        /> 
      </a>

      <a href="https://svelte.dev" target="_blank" rel="noreferrer">
        <img
          src="https://www.svgrepo.com/show/374109/svelte.svg"
          alt="svelte"
          class="icon-badge"
        /> 
      </a>

      <a href="https://www.python.org" target="_blank" rel="noreferrer">
        <img
          src="https://cdn.worldvectorlogo.com/logos/python-5.svg"
          alt="python"
          class="icon-badge"
        />
      </a>
    </p>
   
  </div>

  <h3>{$_('courses')}</h3>
  <ul>
    <li>CS50 Web Programming With Python and Javascript</li>
    <li>Introduction to Typography</li>
    <li>Web Development With React</li>
    <li>Introduction to Software Engineering</li>
    <li>Ideas From the History of Graphic Design</li>
  </ul>

  <br />
  <br />
  <br />
</div>

<style>
  h3 {
    font-size: 2rem;
    border-bottom: 3px solid #efb229;
  }
  p {
    margin-top: -1.3rem;
    margin-bottom: 2.5rem;
  }
  .readme {
    margin-inline: 18rem;
    text-align: left;
  }

  @media (max-width: 900px) {
    .readme {
      margin-inline: 0.5rem;
    }
  }

  .icon-badge {
    width: 70px;
    height: 70px;
  }
 
  .badges {
    padding-block: 2rem;
    padding-inline: 1rem;
    display: flex;
    align-items: center;
    justify-content: space-between;
  }
 
  @media (max-width: 800px) {
    .badges {
      padding-inline: 0.3rem;
      margin-inline: 0.5rem;
    }
    .icon-badge {
      width: 40px;
      height: 40px;
    }
  }
</style>
