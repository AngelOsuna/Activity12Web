<template>
  <div id="app">
    <h1>Chuck Norris Jokes</h1>
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
  text-align: center;
  color: #2c3e50;
  margin-top: 60px;
}

h1 {
  color: #d9534f;
  margin-bottom: 30px;
}
</style>