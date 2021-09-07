<template>
  <span class="anchor" id="about"></span>
  <section class="bg-pine-green">
    <div class="spacer-2 stacked-waves"></div>
    <About/>
  </section>
  
  <div class="spacer layer1"></div>
  <span class="anchor" id="projects"></span>
  <section>
    <Projects/>
    <!-- Projects Component:<br />
    - Slider<br />
    - Project picture<br />
    - Project description<br />
    - Project Component (Modal):<br />
    - images slider<br />
    - link<br />
    - challenges<br />
    - tech stack<br />
    - github link<br /> -->
  </section>

  <div class="spacer layer2"></div>
  <span class="anchor" id="skills"></span>
  <section class="bg-pine-green">
    <Skills/>
  </section>
  
  <div class="spacer layer3"></div>
  <span class="anchor" id="contacts"></span>
  <section>
    <Contacts />
  </section>
</template>

<script setup>
import About from '../components/About.vue'
import Skills from '../components/Skills.vue'
import Contacts from '../components/Contacts.vue'
import Projects from '../components/Projects.vue'

</script>


<style lang="scss" scoped>
.anchor {
  position: absolute;
  transform: translateY(-25vh);
}

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
