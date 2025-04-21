<template>
    <div class="container joke-container">
      <h2 class="text-center mb-5">Chuck Norris Facts</h2>
      <div class="row">
        <chuck-card
          v-for="(joke, index) in jokes"
          :key="index"
          :icon_url="joke.icon_url"
          :value="joke.value"
        />
      </div>
    </div>
  </template>
  
  <script>
  import ChuckCard from './ChuckCard.vue'
  
  export default {
    name: 'JokeList',
    components: {
      ChuckCard
    },
    data() {
      return {
        jokes: [
          { 
            "icon_url": "https://assets.chucknorris.host/img/avatar/chuck-norris.png", 
            "value": "Chuck Norris can skydive into outer space." 
          },
          { 
            "icon_url": "https://assets.chucknorris.host/img/avatar/chuck-norris.png", 
            "value": "The chief export of Chuck Norris is pain." 
          },
          { 
            "icon_url": "https://assets.chucknorris.host/img/avatar/chuck-norris.png", 
            "value": "Chuck Norris doesn't read books. He stares them down until he gets the information he wants." 
          },
          { 
            "icon_url": "https://assets.chucknorris.host/img/avatar/chuck-norris.png", 
            "value": "Time waits for no man. Unless that man is Chuck Norris." 
          },
          { 
            "icon_url": "https://assets.chucknorris.host/img/avatar/chuck-norris.png", 
            "value": "If you spell Chuck Norris in Scrabble, you win. Forever." 
          }
        ]
      }
    }
  }
  </script>
  
  <style scoped>
  .joke-container {
    padding: 20px;
    margin-top: 20px;
  }
  
  h2 {
    color: #d9534f;
    font-weight: bold;
    text-shadow: 1px 1px 2px rgba(0,0,0,0.1);
  }
  </style>