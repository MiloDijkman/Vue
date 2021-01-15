<template>
  <div>
    <div v-bind:key="boodschappen.id" v-for="boodschappen in boodschappen">
      <boodschappenlijst v-bind:boodschappen="boodschappen" />
    </div>
  </div>
</template>

<script>
  import boodschappenlijst from './boodschappenlijst.vue'

export default {
  name: "Boodschappen",
  components: {
    boodschappenlijst
  },
  props: ["boodschappen"]
}
</script>

<style scoped>

</style>
