<template>
  <div id="app">
   <div class="info">
    <h1> James <span> & </span> Alaina</h1>
    <p>This is an ongoing collection of the movies we have watched together from Empire Magazine's list of the 500 greatest movies of all time. </p>
   </div>
    <movies class="movies"></movies>
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
    * {
        box-sizing: border-box;
    }
    
    #app {
        display: flex;
        flex-wrap: wrap;
    }
    body {
        font-family: Roboto, sans-serif;
        font-size: 16px;
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
        width: 100%;
        justify-content: center;
    }
    p {
        margin: 0 auto;
        width: 50%;
    }
    span {
        color: #fda9b8;
    }
    @media only screen and (min-width: 1000px) {
        #app {
            flex-wrap: nowrap;
        }
        body {
            margin: 0 auto;
            max-width: 980px;
        }
        .info {
            flex-direction: column;
            width: 25%;
        }
        .movies {
            width: 75%;
        }
        p {
            width: 100%;
        }
    }
    
</style>
