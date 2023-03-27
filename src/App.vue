<script setup>
  import TheHeader from "./components/TheHeader.vue";
  import TheFooter from "./components/TheFooter.vue";
  import BottomBanner from "./components/BottomBanner.vue";
</script>

<template>
  <TheHeader />

  <div class="container">
    <h3> --> Content goes here <--</h3>
  </div>

  <TheFooter />
  <BottomBanner />
</template>

<style lang="scss">

  @use "./styles/general.scss";

</style>
