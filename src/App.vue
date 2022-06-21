<template>
  <div id="app">
    <TheHeader />
    <TheJumbotron />
    <NavSection />
    <TheFooter />
  </div>
</template>

<script>
import TheHeader from "./components/HeaderPage.vue";
import TheJumbotron from "./components/JumbotronPage.vue";
import NavSection from "./components/SectionNavigation.vue";
import TheFooter from "./components/TheFooter.vue";


export default {
  name: "app",
  components: {TheHeader, TheJumbotron, NavSection, TheFooter, },
}

</script>

<style lang="scss">

</style>
