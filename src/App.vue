<script>
  import AppHeader from '@/components/AppHeader.vue'
  import NavBar from '@/components/NavBar.vue'
  import AppFooter from '@/components/AppFooter.vue'

  export default {
    components: {
      AppHeader,
      NavBar,
      AppFooter,
    }
  }
</script>

<template>
  <div class="container">

    <div class="row">
      <div class="col">
        <app-header />
      </div>
    </div>
    <div class="row">
      <div class="col">
        <nav-bar />
      </div>
    </div>

    <div class="row full-height">
      <!-- <div class="col-3">
        <nav-bar />  
      </div> -->
      <div class="col">
        <router-view />
      </div>
    </div>

    <div class="row">
      <div class="col">
        <app-footer />
      </div>
    </div>

  </div>
</template>

<style>
  * {
    margin: 0;
    padding: 0;
    box-sizing: border-box;
  }
  html, body {
    min-height: 100vh;
  }
  #app {
    min-height: 100vh;
    color: lightgrey;
  }
  .container {
    display: flex;
    flex-direction: column;
    min-height: 100vh;
  }
  .full-height {
    flex: 1
  }
  router-view {
    background-color: yellow;
  }
</style>
