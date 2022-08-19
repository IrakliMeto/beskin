<template>
  <div id="app">
    <TheHeader />
    <router-view />
    <TheFooter />
  </div>
</template>

<style lang="scss">
@import "./assets/styles/main.scss";
</style>
<script>
import TheHeader from "@/components/layout/TheHeader";
import TheFooter from "@/components/layout/TheFooter";

export default {
  components: { TheFooter, TheHeader },
};
</script>
