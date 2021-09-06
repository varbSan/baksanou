<template>
  <Navbar href="home"/>
  <router-view></router-view>
  <footer>Copyright ©2021 by Bak Sanou.</footer>
</template>

<script setup>
import Navbar from './components/Navbar.vue'
import Home from './views/Home.vue'
</script>

<style>
html, body {
  padding: 0;
  margin: 0;
  --color-eeire-black: hsl(0, 0%, 8%);
  --color-ivory: hsl(52, 100%, 97%);
  --color-web-golden: hsl(51, 100%, 50%);
  --color-pine-green: hsl(173, 100%, 21%);
  --color-aero-blue: hsl(167, 90%, 88%);
  --color-polished-pine: hsl(168, 21%, 50%);

  background-color: var(--color-eeire-black);
  scroll-behavior: smooth;
}



#app {
  font-family: Avenir, Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  text-align: center;
  color: var(--color-ivory);

  /* margin-top: 2rem; */
}

footer {
  margin-top: 4rem;
  padding: 2rem 0;
}

</style>
