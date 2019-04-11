<template>
  <div id="app">
    <nav class="nav-links can-hide">
      <router-link class=nav-item to="/">Home</router-link>
      <router-link class=nav-item to="/about">About</router-link>
    </nav>
    <router-view />
  </div>
</template>

<script>
import Skills from './components/Skills.vue'

export default {
  name: 'app',
  components: {
    Skills
  }
}
</script>

<style>
@import url('https://fonts.googleapis.com/css?family=Montserrat:400,700');

body {
  background-color: #EEEEEE;
  font-family: 'Montserrat', sans-serif;
  display: grid;
  grid-template-rows: auto;
  justify-items: center;
  padding-top: 50px;
}
body, html {
  margin: 0;
  height: 100%;
}
.nav-links {
    display: inline-block;
}
.nav-item {
    position: relative;
    display: inline-block;
    margin-left: 1.5rem;
    line-height: 2rem;
}
#app {
    width: 50%;
}
</style>
