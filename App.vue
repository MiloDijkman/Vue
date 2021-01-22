<template>
  <div id="app">
    <Boodschappen v-bind:boodschappen="boodschappen"/>
  </div>
</template>

<script>
import Boodschappen from './components/Boodschappen.vue'

export default {
  name: 'App',
  components: {
    Boodschappen
  },
  data() {
    return {
      boodschappen: [
        {
          id: 1,
          title: "boodschappen een",
          completed: false
        },
        {
          id: 2,
          title: "boodschappen twee",
          completed: true
        },
        {
          id: 3,
          title: "boodschappen drie",
          completed: false
        },
      ]
    }
  }
}
</script>

<style>
* {
  box-sizing: border-box;
  margin: 0;
  padding: 0;
}

body{
  font-family: Arial, Helvetica, sans-serif;
  line-height: 1.4;
}
</style>
