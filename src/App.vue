<template>
  <div id="app">
    <BskHeader />
    <router-view />
    <BskFooter />
  </div>
</template>

<style lang="scss">
@import "./assets/styles/main.scss";
</style>
<script>
import BskHeader from "@/components/layout/BskHeader";
import BskFooter from "@/components/layout/BskFooter";

export default {
  components: { BskFooter, BskHeader },
};
</script>
