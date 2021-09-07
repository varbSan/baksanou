<template>
  <h2 class="title">Contacts</h2>
  <div class="contacts">
    <div class="contact">
      <a href="https://github/varbSan" target="_blank">
        <img class="logo" src="../assets/github-logo.svg" alt="Github">
      </a>
    </div>
    <div class="contact">
      <a href="https://www.linkedin.com/in/bak-sanou-61027b66/" target="_blank">
        <img class="logo" src="../assets/linkedin-logo.svg" alt="LinkedIn">
      </a>
    </div>
    <div class="contact">
      <a href="https://twitter/VarbSan/" target="_blank">
        <img class="logo" src="../assets/twitter-logo.svg" alt="Twitter">
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
  background-color: var(--color-eeire-black);
}
.contacts {
  display: grid;
  grid-template-columns: 1fr;
  align-items: center;
  justify-items: center;

  @media screen and (min-width:600px) {
    grid-template-columns: repeat(3, 1fr);
    padding: 0 4rem;
    margin: 0 auto;
    max-width: 60%;
  } 
  .contact {
    display: grid;
    align-items: center;
    background-color: var(--color-ivory);
    padding: 1rem;
    margin: .5rem;
    border-radius: 50%;
    transition: all 200ms;
    &:hover {
      @media screen and (hover:hover) {
        transform: scale(1.1);
        box-shadow:  0rem 0rem 4px var(--color-ivory);
      }      
    }
    a {
      .logo {
        width: 4rem;
      }
    }
  }
}
</style>
