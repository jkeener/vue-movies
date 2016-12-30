<template>
  <div id="app">
    <h1>{{ title }}</h1>
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
      title: "James & Alaina's Movies"
    }
  }
}
</script>

<style>
    body {
        font-family: Roboto;
    }
    #app {
        display: flex;
    }
</style>
