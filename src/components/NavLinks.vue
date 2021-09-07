<template>
  <div class="links">
    <div>
      <a href="#about">About</a>
    </div>
    <div>
      <a href="#projects">Projects</a>
    </div>
    <div>
      <a href="#skills">Skills</a>
    </div>
    <!-- <div>
      <a href="#experience">Experience</a>
    </div> -->
    <div>
      <a href="#contacts">Contact</a>
    </div>
  </div>
</template>

<script setup>

</script>

<style lang="scss" scoped>

  .links {
    margin-left: auto;
    text-align: center;
    display: flex;
    div{
      min-width: 5rem;

      a {
        font-size: 0.8rem;
        overflow: hidden;
        color: inherit;
        text-decoration: none;
        transition: all 200ms;

        @media screen and (min-width: 600px) {
          &:hover {
            font-weight: bold;
            transform: scale(1.1);
            text-shadow:  0rem 0rem 1px var(--color-ivory);
          }          
        }
      }
    }

  }

  @media screen and (max-width: 600px) {
    .links {
      display: inline-block;
    }
  }
</style>
