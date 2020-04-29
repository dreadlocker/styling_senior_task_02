<template>
  <div id="app">
    <MainComponent />
  </div>
</template>

<script>
import MainComponent from "./components/MainComponent.vue";

export default {
  name: "App",
  components: {
    MainComponent
  }
};
</script>

<style lang="sass">
@import "@/assets/SASS/styles.sass"

#app
  font-family: Avenir, Helvetica, Arial, sans-serif
  -webkit-font-smoothing: antialiased
  -moz-osx-font-smoothing: grayscale
  text-align: center
</style>
