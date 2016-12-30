<template>
  <div id="app">
   <div class="info">
    <h1> James <span> & </span> Alaina</h1>
    <p>This is an ongoing collection of the movies we have watched together from Empire Magazine's list of the 500 greatest movies of all time. </p>
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
        flex-direction: column;
        margin-left: .5em;
    }
    
    h1 {
        font-family: 'Reem Kufi', sans-serif;
        font-size: 3em;
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
