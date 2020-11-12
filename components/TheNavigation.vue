<template>
  <nav class="navbar has-shadow is-transparent" role="navigation" aria-label="main navigation">
    <div class="container is-max-widescreen">
      <div class="navbar-brand">            
        <b-button type="is-outlined">
          <b-icon icon="github"></b-icon>              
          <span><a href="https://github.com/IngridAmprou/" target="_blank">View source</a></span>
        </b-button>
        <a
          role="button"
          class="navbar-burger burger"
          aria-label="menu"
          aria-expanded="false"
          @click="showMenu = !showMenu"
          :class="{ 'is-active' : showMenu }"            
        >
        <span aria-hidden="true"></span>
        <span aria-hidden="true"></span>
        <span aria-hidden="true"></span>
        </a>
      </div>
      <div class="navbar-menu" :class="{ 'is-active' : showMenu }">
        <div class="navbar-end">
          <nuxt-link to="/" class="navbar-item"><a>Home</a></nuxt-link>
          <nuxt-link to="/work" class="navbar-item"><a>Work</a></nuxt-link>      
        </div>   
      </div>
    </div>
  </nav>  

</template>

<script>
export default {
  data() {
    return {
      showMenu: false
    };
  }
};
</script>

<style lang="scss" scoped>
.button {
  margin-top: 0.4em;
  margin-left: 0.4em;
}
.icon {
 color: $black;
}
.navbar-end {
  list-style: none;
}
.navbar-burger.burger {
 color: $black;
 background-color: transparent;
}
.navbar-item {
  display: flex;
  align-items: center;
  justify-content: center;
}
</style>