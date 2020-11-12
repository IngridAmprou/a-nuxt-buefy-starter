<template>
  <div>
    <TheHeader />
      <div class="hero is-primary is-large is-bold css-pattern-component">
        <nuxt />
        <TheFooter />
      </div>
  </div>  
</template>

<script>
import TheHeader from '~/components/TheHeader.vue';
import TheFooter from '~/components/TheFooter.vue'

export default {
  components: {
    TheHeader,
    TheFooter,
  }
}
</script>

<style lang="scss">
html {
  -ms-text-size-adjust: 100%;
  -webkit-text-size-adjust: 100%;
  -moz-osx-font-smoothing: grayscale;
  -webkit-font-smoothing: antialiased;
  box-sizing: border-box;
}
.css-pattern-component {
  background-image: linear-gradient(45deg, transparent 20%, black 50%, transparent 20%),
                    radial-gradient(rgba(241,241,241, 0.6) 1px, transparent 0);
  background-size: 3px 3px, 3px 1px;
}
::-moz-selection{
    background-color:#EE0000;
    }
::selection{
    background-color: #EE0000;
    }
</style>
