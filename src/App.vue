<template>
  <div id="app">
    <TheHeader />
    <TheJumbotron />
    <NavSection />
    <TheFooter />
    <BannerSignUp />
  </div>
</template>

<script>
import TheHeader from "./components/HeaderPage.vue";
import TheJumbotron from "./components/JumbotronPage.vue";
import NavSection from "./components/SectionNavigation.vue";
import TheFooter from "./components/TheFooter.vue";
import BannerSignUp from "./components/BannerSignUp.vue"


export default {
  name: "app",
  components: {TheHeader, TheJumbotron, NavSection, TheFooter, BannerSignUp},
}

</script>

<style lang="scss">

@import "~bootstrap/scss/bootstrap";

</style>
