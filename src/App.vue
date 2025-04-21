<template>
  <div id="app">
    <JokeList />
  </div>
</template>

<script>
import JokeList from './components/JokeList.vue'

export default {
  name: 'App',
  components: {
    JokeList
  }
}
</script>

<style>
#app {
  font-family: Avenir, Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  min-height: 100vh;
  background-color: #f8f9fa;
}
</style>