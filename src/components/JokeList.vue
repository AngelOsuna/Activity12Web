<template>
    <div class="joke-container">
      <ul class="joke-list">
        <li v-for="(joke, index) in jokes" :key="index" class="joke-item">
          {{ joke.value }}
        </li>
      </ul>
    </div>
  </template>
  
  <script>
  export default {
    name: 'JokeList',
    data() {
      return {
        jokes: [
          { "value": "Chuck Norris can skydive into outer space." },
          { "value": "The chief export of Chuck Norris is pain." },
          { "value": "Chuck Norris doesn't read books. He stares them down until he gets the information he wants." },
          { "value": "Time waits for no man. Unless that man is Chuck Norris." },
          { "value": "If you spell Chuck Norris in Scrabble, you win. Forever." }
        ]
      }
    }
  }
  </script>
  
  <style scoped>
  .joke-container {
    max-width: 800px;
    margin: 0 auto;
    padding: 20px;
  }
  
  .joke-list {
    list-style-type: none;
    padding: 0;
  }
  
  .joke-item {
    background-color: #f9f9f9;
    border-left: 5px solid #d9534f;
    margin: 10px 0;
    padding: 15px;
    border-radius: 0 5px 5px 0;
    box-shadow: 0 2px 5px rgba(0,0,0,0.1);
    transition: transform 0.2s;
  }
  
  .joke-item:hover {
    transform: translateX(5px);
    background-color: #f1f1f1;
  }
  </style>