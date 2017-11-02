<template>
<div class="heading">
  <h1> James <span> & </span> Alaina</h1>
  <p>This is an ongoing collection of the movies we have watched together from Empire Magazine's list of the 500 greatest movies of all time. </p>
</div>
</template>

<script>
export default {
  data() {
    return {

    }
  }
}
</script>

<style>

@import url('https://fonts.googleapis.com/css?family=Reem+Kufi');

.heading {
  margin-bottom: 1em;
  display: flex;
  flex-direction: column;
  align-items: center;
  justify-content: center;
  padding: 1em;
}

h1 {
  font-family: 'Reem Kufi', sans-serif;
  font-size: 2.89em;
}

p {
  padding: 1em;
  width: 90%
}

@media screen and (min-width: 800px) {
  p {
    width: 60%
  }
}

@media screen and (min-width: 1100px) {
  .heading {
    width: 30%;
    align-self: flex-start;
    position: sticky;
    top: 0;
    margin: 0;
  }
  p {
    width: 90%
  }
}

</style>
