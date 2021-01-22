<template>
  <div>
    <div v-bind:key="boodschappen.id" v-for="boodschappen in boodschappen">
      <Boodschappen v-bind:boodschappen="boodschappen" />
    </div>
  </div>
</template>

<script>
import BoodschappenItem from './boodschappenlijst.vue';

export default {
  name: "Boodschappen",
  components: {
    BoodschappenItem
  },
  props: ["boodschappen"]
}
</script>

<style scoped>

</style>
