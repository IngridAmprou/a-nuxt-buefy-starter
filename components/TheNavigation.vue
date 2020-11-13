<template>
  <b-navbar class="navbar has-shadow is-transparent" role="navigation" aria-label="main navigation">
    <template slot="brand">
      <b-navbar-item>
        <b-button type="is-outlined">
          <b-icon icon="github"></b-icon>              
          <span><a href="https://github.com/IngridAmprou/a-nuxt-buefy-starter" target="_blank">View source</a></span>
        </b-button>
      </b-navbar-item>
    </template>      
    <template slot="end">
      <b-navbar-item tag="nuxt-link" to="/">About</b-navbar-item>
      <b-navbar-item tag="nuxt-link" to="/portfolio">Portfolio</b-navbar-item>
    </template>
  </b-navbar>   
</template>

<style lang="scss" scoped>
.icon {
 color: $black;
}
.navbar-item {
  color: $black;
  display: flex;
  align-items: center;
  justify-content: center;
}
a.navbar-item:hover {
  color: #EE0000;
}  
</style>