<template>
  <div id="app">
   <div class="info">
    <h1> James <span> & </span> Alaina</h1>
    <p>This is an ongoing collection of the movies we have watched together</p>
   </div>
    <movies></movies>
  </div>
</template>

<script>

import movies from './Movies.vue'

export default {
    components: {
    movies
  },
  name: 'app',
  data () {
    return {
        
    }
  }
}
</script>

<style>
    
    @import url('https://fonts.googleapis.com/css?family=Reem+Kufi');
    
    #app {
        display: flex;
    }
    
    body {
        font-family: Roboto, sans-serif;
    }
    
    .info {
        display: flex;
        display: flex;
        margin: 0;
    }
    
    p {
        margin: 0;
    }
    
    span {
        color: #fda9b8;
    }
    
</style>
