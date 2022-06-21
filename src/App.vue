<template>
  <div id="app">
    <TheHeader />
    <TheJumbotron />
  </div>
</template>

<script>
import TheHeader from "./components/HeaderPage.vue";
import TheJumbotron from "./components/JumbotronPage.vue"


export default {
  name: "app",
  components: {TheHeader, TheJumbotron},
}

</script>

<style lang="scss">

</style>
