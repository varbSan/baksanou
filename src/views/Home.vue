<template>
  <section class="bg-pine-green" id="about">
    <div class="spacer-2 stacked-waves"></div>
    <About/>
  </section>
  <div class="spacer layer1"></div>

  <section id="projects">
    Projects Component:<br />
    - Slider<br />
    - Project picture<br />
    - Project description<br />
    - Project Component (Modal):<br />
    - images slider<br />
    - link<br />
    - challenges<br />
    - tech stack<br />
    - github link<br />
  </section>

  <div class="spacer layer2"></div>
  <section class="bg-pine-green" id="skills">
    <Skills/>
  </section>
  <div class="spacer layer3"></div>

  <section id="contact">
    Contact Component:<br />
    - LinkedIn<br />
    - Twitter<br />
  </section>
</template>

<script setup>
import About from '../components/About.vue'
import Skills from '../components/Skills.vue'

</script>


<style lang="scss" scoped>

.spacer {
  aspect-ratio: 960/300;
  background-repeat: no-repeat;
  background-position: center;
  background-size: cover;
}

.spacer-2 {
  height: 16vh;
  background-repeat: no-repeat;
  background-position: bottom;
  background-size: cover;
}

.stacked-waves {
  background-image: url('../assets/stacked-waves.svg');
  // overflow: visible;
}
.layer1 {
  background-image: url('../assets/layered-waves-1.svg');
}
.layer2 {
  background-image: url('../assets/layered-waves-2.svg');
}
.layer3 {
  background-image: url('../assets/layered-waves-3.svg');
}


.bg-pine-green {
  background-color: var(--color-pine-green);
}

</style>
