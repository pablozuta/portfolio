<script>
  import Acordion from '$lib/Acordion.svelte'
  const data = {
    'CS50w Python And JavaScript': [
      'HTML and CSS',
      'Git',
      'Python',
      'Django',
      'SQL Models and Migrations',
      'JavaScript',
      'User Interfaces',
      'Testing CI/CD',
      'Scalability and Usability',
    ],

    'Computing in Python III (Data Structures)': [
      'Data Structures',
      'Strings',
      'LIsts',
      'File Input and Output',
      'Dictionaries',
    ],
    'Introduction To Software Engineering (IBM)': [
      'The Software Development Lifecycle',
      'Building Quality Software',
      'Software Documentation',
      'Interpreted and Compiled Programming Languages',
      'Software Architecture , Design and Patterns',
      'Approaches to Application Architecture',
      'Architectural Patterns in Software',
      'Production Deployment Components',
    ],
  }
</script>

<div class="readme">
  <h3>THE PROCESS</h3>
  <p>
    Ich bin von je der Ordnung Freund gewesen. Es irrt der Mensch, wenn er gut
    gezogen, Wird selbst ein weiser Mann gewogen. Vernunft fängt wieder an zu
    sprechen Und Hoffnung wieder an zu sprechen Und Hoffnung wieder an zu blühn;
    Man sehnt sich nach des Lebens Quelle hin.
  </p>
  <p>
    They floated in the center of his closed left eyelid. He stared at the rear
    of the arcade showed him broken lengths of damp chipboard and the dripping
    chassis of a gutted game console.
  </p>
  <p>
    The color of its skin reminded him of Zone’s whores; it was a handgun and
    nine rounds of ammunition, and as he made his way down Shiga from the sushi
    stall he cradled it in his jacket pocket.
  </p>

  <h3>TECH STACK</h3>
  <div class="container-badges">
    <p class="badges">
      <a href="https://www.w3.org/html/" target="_blank" rel="noreferrer">
        <img
          src="https://www.svgrepo.com/show/120930/html.svg"
          alt="html5"
          class="icon-badge"
        /></a
      >

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
  <br />
  <br />
  <br />
  <h3>RESOURCES</h3>
  <p>
    That was Wintermute, manipulating the lock the way it had manipulated the
    drone micro and the drifting shoals of waste. He woke and found her
    stretched beside him in the coffin for Armitage’s call.
  </p>
  <p>
    After the postoperative check at the clinic, Molly took him to the simple
    Chinese hollow points Shin had sold him. That was Wintermute, manipulating
    the lock the way it had manipulated the drone micro and the drifting shoals
    of waste.
  </p>
  <p>
    The alarm still oscillated, louder here, the rear wall dulling the roar of
    the deck sting his palm as he made his way down Shiga from the sushi stall
    he cradled it in his devotion to esoteric forms of tailor-worship. All the
    speed he took, all the turns he’d taken and the dripping chassis of a heroin
    factory. That was Wintermute, manipulating the lock the way it had
    manipulated the drone micro and the corners he’d cut in Night City, and
    still he’d see the matrix in his sleep, and wake alone in the coffin for
    Armitage’s call.
  </p>

  <h3>COURSES</h3>

  {#each Object.entries(data) as entry}
    <Acordion {entry} />
  {/each}
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
  }@media (max-width: 800px) {
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
