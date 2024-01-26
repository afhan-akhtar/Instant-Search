<template>
  <div id="app">
    <img alt="Vue logo" src="./assets/logo.png">
    <InstantSearch />
  </div>
</template>

<script>
import InstantSearch from './components/InstantSearch.vue'

export default {
  name: 'App',
  components: {
    InstantSearch
  }
}
</script>

<style>
#app {
  font-family: Avenir, Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  text-align: center;
  color: #2c3e50;
  margin-top: 60px;
}

.centered-list {
  list-style: none;
  padding: 0;
  text-align: center;
}

.centered-list li {
  margin: 10px 0;
  /* Adjust the margin as needed */
}
</style>

