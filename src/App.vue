<template>
  <div id="app">
    <TheHeader />
    <TheJumbotron />
    <NavSection />
  </div>
</template>

<script>
import TheHeader from "./components/HeaderPage.vue";
import TheJumbotron from "./components/JumbotronPage.vue";
import NavSection from "./components/SectionNavigation.vue"


export default {
  name: "app",
  components: {TheHeader, TheJumbotron, NavSection},
}

</script>

<style lang="scss">

</style>
