<template>
  <div>
    <TheBanner />

    <div class="content">
      <div class="container padding content__inner">
        <TheProvider />
        <TheAbout />
      </div>
    </div>

    <CardsContainer />
    <TheDescription />
    <PropertiesBlock />
  </div>
</template>

<script>
import TheAbout from "@/components/TheAbout";
import TheBanner from "@/components/banner/TheBanner";
import TheProvider from "@/components/TheProvider";
import CardsContainer from "@/components/CardsContainer";
import TheDescription from "@/components/TheDescription";
import PropertiesBlock from "@/components/PropertiesBlock";

export default {
  name: "HomeView",
  components: {
    PropertiesBlock,
    TheDescription,
    CardsContainer,
    TheAbout,
    TheProvider,
    TheBanner,
  },
};
</script>

<style lang="scss" scoped>
.content {
  width: 100%;
  padding: 120px 0;
  background-color: #fff;

  @media (max-width: 767px) {
    padding: 60px 0;
  }
}
</style>
