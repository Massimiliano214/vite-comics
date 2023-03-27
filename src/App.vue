<script setup>
  import TheHeader from "./components/TheHeader.vue";
  import TheFooter from "./components/TheFooter.vue";
  import BottomBanner from "./components/BottomBanner.vue";
  import MainBanner from "./components/MainBanner.vue";
</script>

<template>
  <TheHeader />
  <main>
    <div class="container">
      <h3>  -- &gt; Content goes here &lt;--  </h3>
    </div>
  </main>
  

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
