<template>
  <h2 class="title">Projects</h2>
  <div class="projects">
    <div class="project">
      <a href="https://everydaycarry-land.web.app/" target="_blank">
        <img class="screenshot" src="../assets/screenshots/ss-edc-land.png" alt="Everyday Carry Land"><br>
        <span class="project-date">2021</span>
        <h3 class="project-name">Everyday Carry Land</h3>
        <p class="project-description">
          The most complex project I've built regarding routing. I had to build "auth guards" to manage permission between visitors. Only signed up users can access the full website. Only the owner of a post can delete it etc.
        </p>
        <p class="techstack">
          <img class="techstack-logo" src="../assets/logos/logo-vue.svg">
          <img class="techstack-logo" src="../assets/logos/logo-firebase.svg">
          <img class="techstack-logo" src="../assets/logos/logo-Sass.svg">
          <img class="techstack-logo" src="../assets/logos/logo-vite.svg">
        </p>
      </a>
    </div>
    <div class="project">
      <a href="https://breath-room.web.app/" target="_blank">
        <img class="screenshot" src="../assets/screenshots/ss-breath-room.png" alt="Breath Room"><br>
        <span class="project-date">2021</span>
        <h3 class="project-name">Breath Room</h3>
        <p class="project-description">
          This project was a good pretext to learn Vue 3 and ViteJS. I already knew Vue 2 but was very enthusiast about the new composition API.
        </p>
        <p class="techstack">
          <img class="techstack-logo" src="../assets/logos/logo-vue.svg">
          <img class="techstack-logo" src="../assets/logos/logo-firebase.svg">
          <img class="techstack-logo" src="../assets/logos/logo-Sass.svg">
          <img class="techstack-logo" src="../assets/logos/logo-vite.svg">
        </p>
      </a>
    </div>
  
    <div class="project">
      <a href="https://donquixote.land/" target="_blank">
        <img class="screenshot" src="../assets/screenshots/ss-donquixote-land.png" alt="Don Quixote Land"><br>
        <span class="project-date">2021</span>
        <h3 class="project-name">Don Quixote Land</h3>
        <p class="project-description">
          This project was clearly a way to improve my CSS and Sass skills. The website has no purpose except to show how it is perfectly responsive and animated on every device.
        </p>
        <p class="techstack">
          <img class="techstack-logo" src="../assets/logos/logo-html.svg">
          <img class="techstack-logo" src="../assets/logos/logo-css.svg">
          <img class="techstack-logo" src="../assets/logos/logo-Sass.svg">
        </p>
      </a>
    </div>
    <div class="project">
      <a href="https://chrome.google.com/webstore/detail/overview-personal-roadmap/bnacpnpmhffilkifmaahoabkgpkblcnl" target="_blank">
        <img class="screenshot" src="../assets/screenshots/ss-overview.png" alt="Over[v]iew"><br>
        <span class="project-date">2020</span>
        <h3 class="project-name">Over[v]iew</h3>
        <p class="project-description">
          My masterpiece so far. Although it doesn't look like much, making a Vue.js app run in a chrome extension environnement is not that easy. Protocols are different, and fetching data from the Google APIs was a real challenge.<br>I use Over[v]iew on a daily basis, along with my users.
        </p>
        <p class="techstack">
          <img class="techstack-logo" src="../assets/logos/logo-vue.svg">
          <img class="techstack-logo" src="../assets/logos/logo-firebase.svg">
          <img class="techstack-logo" src="../assets/logos/logo-webpack.svg">
        </p>
      </a>
    </div>
    <div class="project">
      <a href="https://citizencult.com/" target="_blank">
        <img class="screenshot" src="../assets/screenshots/ss-citizencult.png" alt="Citizen Cult"><br>
        <span class="project-date">2019</span>
        <h3 class="project-name">Citizen Cult</h3>
        <p class="project-description">
          My very first project. I built everything from the ground up to get good fundamentals before learning a frontend framework. Also I used Node and its framework Express to introduce myself to backend development.
        </p>
        <p class="techstack">
          <img class="techstack-logo" src="../assets/logos/logo-html.svg">
          <img class="techstack-logo" src="../assets/logos/logo-css.svg">
          <img class="techstack-logo" src="../assets/logos/logo-javascript.svg">
          <img class="techstack-logo" src="../assets/logos/logo-nodejs.svg">
          <img class="techstack-logo" src="../assets/logos/logo-express.svg">
          <img class="techstack-logo" src="../assets/logos/logo-mongodb.svg">
          <img class="techstack-logo" src="../assets/logos/logo-heroku.svg">
        </p>
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
}
.projects {
  display: grid;
  padding: 0 1rem;
  justify-content: center;
  grid-template-columns: repeat(auto-fit, minmax(20rem, 1fr));
  grid-gap: 1rem;
  @media screen and (min-width: 600px){
    padding: 0 3rem;
  }
  .project {
    display: grid;
    align-items: start;
    background-color: hsla(0, 0%,100%, 10%);
    padding: .5rem;
    margin: .5rem;
    border-radius: .5rem;
    min-height: 6rem;
    transition: all 200ms;
    box-shadow: 0rem 0rem .5rem var(--color-pine-green);

    @media screen and (min-width: 600px) {
      &:hover {
        transform: scale(1.02);
        box-shadow: 0rem 0rem 1rem var(--color-polished-pine);
      }      
    }

    &-description {
      font-size: .7rem;
      text-align: left;
      padding: 0 1rem;
      font-weight: 400;
    }

    &-date {
      background-color: hsla(0, 0%,100%, 20%);
      color: var(--color-eeire-black);
      padding: .2rem;
      border-bottom-left-radius: .2rem;
      border-bottom-right-radius: .2rem;
    }
    a {
      font-size: 0.8rem;
      overflow: hidden;
      color: inherit;
      font-weight: bold;
      text-decoration: none;

      .screenshot {
        width: 100%;
        border-radius: .5rem;
      }
    }
    .techstack {
      &-logo {
        width: 1.5rem;
        padding: 0 .2rem;
      }
    }
  }
}
</style>
