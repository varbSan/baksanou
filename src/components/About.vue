<template>
  <div class="about">
    <Blob class="blob"/> 
    <div class="presentation">
      <h3>Hi, I'm Bakary</h3>
      <transition name="slide-fade">
        <h2>{{proTitle.title}}</h2>
      </transition>
      <p>
        I thrive working with the Vue.js framework and its ecosystem. 💚<br>
        That said, I identify as a variable developer. I am willing to work with any technology! 
      </p>
      <p>
        If you like this portfolio, reach out to me on <a href="https://www.linkedin.com/in/bak-sanou-61027b66/" target="_blank">Linkedin</a>.
        <br>I am always available for a good chat. 😉
      </p>
    </div>
  </div>
</template>

<script setup>
import { ref } from '@vue/reactivity'
import { onMounted } from '@vue/runtime-core'
import Blob from '../components/Blob.vue'

const proTitles = ref(['Web Developer', 'Constant Learner', 'Vue.js Enthusiast'])
const proTitle = ref({title:'Web Developer', index:0})

let count = 0
setInterval(() => {
  proTitles.value.forEach((title , index) => {
    if(index === count) {
      proTitle.value.title = title 
      proTitle.value.index = index
    }
  })
  count++
  if(count >= proTitles.value.length ) {
    count = 0
  }
}, 2000)

</script>

<style lang="scss" scoped>

.about {
  display: grid;
  grid-template-columns: repeat(auto-fit, minmax(20rem, 1fr));
  align-items: center;
  justify-items: center;
  padding-top: -3rem;
  .presentation {
    text-align: left;
    padding: 0 2rem;
    h2 {
      font-size: 3rem;
      margin: 1.5rem 0;
    }

    a {
      text-decoration: underline;
      color: inherit;
      font-weight: bold;
      transition: all 100ms;
      &:hover {
        text-shadow:  0rem 0rem 1px var(--color-ivory);
      }
    }

  }
}
</style>
