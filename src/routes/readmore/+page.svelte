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
  <h3>THE JOURNEY</h3>
  <p>
    As a self-taught web developer, I have experienced both the rewards and
    challenges of learning this field on my own. It has required a lot of
    dedication and motivation to learn the various technologies and concepts,
    and there have been times when I have felt frustrated or overwhelmed.
  </p>
  <p>
    However, I have found that the key to success is to start with a good
    resource, such as a tutorial or online course, that covers the basics of
    HTML, CSS, and JavaScript. These are the foundational technologies for
    building websites and web applications, and it's important to have a solid
    understanding of them before moving on to more advanced topics.
  </p>
  <p>
    As I progressed through my learning, I found it helpful to practice my
    skills by building small projects or websites. This gave me a sense of what
    it's like to work on a real-world project and also allowed me to show my
    work to potential employers or clients.
  </p>
  <p>
    One of the biggest challenges I faced as a self-taught web developer was
    staying motivated and on track. It can be easy to get discouraged or lose
    focus, especially when you're learning on your own. To stay motivated, I set
    small, achievable goals for myself and celebrated my progress along the way.
    I also connected with other self-taught developers and joined online
    communities to get support and encouragement.
  </p>
  <p>
    I am also willing to try new things and take on new challenges, even if I
    don't have a lot of experience in a particular area. I know that the best
    way to learn is to get hands-on experience and make mistakes, and I am
    always looking for opportunities to do so. Overall, my willingness to keep
    learning and growing as a web developer has helped me to become a better
    developer and to take on more complex and rewarding projects. I am excited
    to see where my learning journey will take me next.
  </p>
  <br>
  <br>

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
