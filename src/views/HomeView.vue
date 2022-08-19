<template>
  <div>
    <BskBanner />

    <div class="content">
      <div class="container padding content__inner">
        <BskProvider />
        <BskAbout />
      </div>
    </div>

    <CardsContainer />
    <BskDescription />
    <PropertiesBlock />
  </div>
</template>

<script>
import BskAbout from "@/components/BskAbout";
import BskBanner from "@/components/banner/BskBanner";
import BskProvider from "@/components/BskProvider";
import CardsContainer from "@/components/CardsContainer";
import BskDescription from "@/components/BskDescription";
import PropertiesBlock from "@/components/PropertiesBlock";

export default {
  name: "HomeView",
  components: {
    PropertiesBlock,
    BskDescription,
    CardsContainer,
    BskAbout,
    BskProvider,
    BskBanner,
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
