<template>
  <div class="navbar" id="navbar">
    <nav>
      <div class="title" @click="goTop" href="#navbar">
        <!-- <img src="../assets/logos/logo-variable.svg" alt="" width="60"/> -->
        <h1>BS</h1>
      </div>
      <NavLinks/>
      <!-- <DropdownMenu/> -->
    </nav>
  </div>
</template>

<script setup>
import NavLinks from '../components/NavLinks.vue'

function goTop() {
  window.scrollTo(0, 0)
}
window.onscroll = function() {scrollFunction()};
 
function scrollFunction() {
  if (document.body.scrollTop > 20 || document.documentElement.scrollTop > 20) {
    
    document.getElementById("navbar").style.background = "var(--color-eeire-black)";
  } else {
   
    document.getElementById("navbar").style.background = "none";
  }
}

</script>

<style lang="scss" scoped>
.navbar {
  text-align: left;
  position: fixed;
  width: 100%;
  z-index: 1000;
  transition: 1000ms;
}

.title {

  display: flex;
  transition: all 200ms;
  cursor: pointer;
  text-decoration-line: overline underline;
  text-underline-offset: 4px;
  &:hover, &active {
    font-weight: bolder;
    text-shadow:  0rem 0rem 1px var(--color-ivory);
    transform:scale(1.05)
  }
}


nav {
  display: flex;
  align-items: center;
  // max-width: 120rem;
  margin: 0 auto;
  padding: 1rem .8rem;


  h1 {
    margin-left: 1.2rem;
    margin-top: .5rem;
    margin-bottom: .5rem;

    align-items: center;
  }


}
</style>
