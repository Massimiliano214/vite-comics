<script>
  import TheHeader from "./components/TheHeader.vue";
  import TheFooter from "./components/TheFooter.vue";
  import BottomBanner from "./components/BottomBanner.vue";
  import MainBanner from "./components/MainBanner.vue";
  import MainHub from "./components/MainHub.vue";

  export default {
    components: {
      TheHeader,
      TheFooter,
      BottomBanner,
      MainBanner,
      MainHub
    }
  }
</script>

<template>
  <TheHeader />
  <MainHub />
  <MainBanner />
  <TheFooter />
  <BottomBanner />
</template>

<style lang="scss">

  @use "./styles/general.scss";

  main {
    background-color: rgb(34, 34, 34);
    height: 150px;
    color: white;
  }


</style>
