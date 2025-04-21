<template>
    <div class="col-md-4 col-sm-6 col-12 mb-4">
      <div class="card h-100">
        <img :src="icon_url" class="card-img-top" alt="Chuck Norris">
        <div class="card-body">
          <p class="card-text">{{ value }}</p>
        </div>
      </div>
    </div>
  </template>
  
  <script>
  export default {
    name: 'ChuckCard',
    props: {
      icon_url: {
        type: String,
        required: true
      },
      value: {
        type: String,
        required: true
      }
    }
  }
  </script>
  
  <style scoped>
  .card {
    border: 2px solid #d9534f;
    border-radius: 10px;
    transition: transform 0.3s;
  }
  
  .card:hover {
    transform: translateY(-5px);
    box-shadow: 0 10px 20px rgba(0,0,0,0.1);
  }
  
  .card-img-top {
    padding: 20px;
    background-color: #f8f9fa;
    border-bottom: 1px solid rgba(0,0,0,.125);
  }
  
  .card-text {
    font-style: italic;
  }
  </style>