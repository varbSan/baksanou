<template>
  <h2 class="title">Skills</h2>
  <div class="skills">
    <div class="skill">
      <a href="https://262.ecma-international.org/6.0/" target="_blank">
        <img class="logo" src="../assets/logos/logo-javascript.svg" alt="JavaScript"><br>
        <span class="skill-name">JavaScript:<br>ES6/ES2015+</span>
      </a>
    </div>
    <div class="skill">
      <a href="https://html.spec.whatwg.org/multipage/" target="_blank">
        <img class="logo" src="../assets/logos/logo-html.svg" alt="HTML 5"><br>
        <span class="skill-name">HTML 5</span>
      </a>
    </div>
    <div class="skill">
      <a href="https://developer.mozilla.org/en-US/docs/Web/CSS" target="_blank">
        <img class="logo" src="../assets/logos/logo-css.svg" alt="CSS 3"><br>
        <span class="skill-name">CSS 3:<br>Grid • Flexbox</span>
      </a>
    </div>
    <div class="skill">
      <a href="https://sass-lang.com/" target="_blank">
        <img class="logo" src="../assets/logos/logo-sass.svg" alt="Sass"><br>
        <span class="skill-name">Sass:<br>Scss</span>
      </a>
    </div>
    <div class="skill">
      <a href="https://v3.vuejs.org/" target="_blank">
        <img class="logo" src="../assets/logos/logo-vue.svg" alt="Vue.js"><br>
        <span class="skill-name">Vue 2 & 3:<br>Vuex • Vue Router • Vuetify</span>
      </a>
    </div>
    <div class="skill">
      <a href="https://expressjs.com/" target="_blank">
        <img class="logo" src="../assets/logos/logo-express.svg" alt="Express.js"><br>
        <span class="skill-name">Express.js</span>
      </a>
    </div>
    <div class="skill">
      <a href="https://mongodb.com/" target="_blank">
        <img class="logo" src="../assets/logos/logo-mongodb.svg" alt="MongoDB"><br>
        <span class="skill-name">MongoDB</span>
      </a>
    </div>
    <div class="skill">
      <a href="https://firebase.google.com/" target="_blank">
        <img class="logo" src="../assets/logos/logo-firebase.svg" alt="Google Firebase"><br>
        <span class="skill-name">Firebase:<br>Firestore • Hosting • Auth • Storage</span>
      </a>
    </div>
    <div class="skill">
      <a href="https://mysql.com/" target="_blank">
        <img class="logo" src="../assets/logos/logo-mysql.svg" alt="MySQL"><br>
        <span class="skill-name">MySQL</span>
      </a>
    </div>
    <div class="skill">
      <a href="https://www.heroku.com/" target="_blank">
        <img class="logo" src="../assets/logos/logo-heroku.svg" alt="Heroku"><br>
        <span class="skill-name">Heroku</span>
      </a>
    </div>
    <div class="skill">
      <a href="https://www.github.com/" target="_blank">
        <img class="logo" src="../assets/logos/logo-github.svg" alt="Github"><br>
        <span class="skill-name">Github</span>
      </a>
    </div>
    <div class="skill">
      <a href="https://www.git-scm.com/" target="_blank">
        <img class="logo" src="../assets/logos/logo-git.svg" alt="Git"><br>
        <span class="skill-name">Git</span>
      </a>
    </div>
    <div class="skill">
      <a href="https://www.nodejs.org/" target="_blank">
        <img class="logo" src="../assets/logos/logo-nodejs.svg" alt="Node.js"><br>
        <span class="skill-name">Node.js</span>
      </a>
    </div>
    <div class="skill">
      <a href="https://www.npmjs.com/" target="_blank">
        <img class="logo" src="../assets/logos/logo-npm.svg" alt="npm"><br>
        <span class="skill-name">npm</span>
      </a>
    </div>
    <div class="skill">
      <a href="https://www.vitejs.dev/" target="_blank">
        <img class="logo" src="../assets/logos/logo-vite.svg" alt="Vite JS"><br>
        <span class="skill-name">ViteJS</span>
      </a>
    </div>
    <div class="skill">
      <a href="https://www.webpack.js.org/" target="_blank">
        <img class="logo" src="../assets/logos/logo-webpack.svg" alt="Webpack js"><br>
        <span class="skill-name">Webpack</span>
      </a>
    </div>

  </div>
</template>

<script setup>

</script>

<style lang="scss" scoped>

.title {
  margin: 0;
  padding: 2rem 0;
  background-color: var(--color-pine-green);
}
.skills {
  display: grid;
  grid-template-columns: repeat(auto-fit, minmax(10rem, 1fr));

  @media screen and (min-width:600px) {
    padding: 0 4rem;
  } 
  .skill {
    display: grid;
    align-items: center;
    background-color: hsla(0, 0%,100%, 25%);
    padding: .5rem;
    margin: .5rem;
    border-radius: 1rem;
    min-height: 6rem;
    transition: all 200ms;
    &:hover {
      @media screen and (hover:hover) {
        transform: scale(1.05) rotate(-2deg);
        box-shadow: 0rem 0rem 5px var(--color-aero-blue);
        text-shadow:  0rem 0rem 1px var(--color-ivory);
      }      
    }
    a {
      font-size: 0.8rem;
      overflow: hidden;
      color: inherit;
      font-weight: bold;
      text-decoration: none;

      .logo {
        width: 3rem;
      }
    }
  }
}
</style>
