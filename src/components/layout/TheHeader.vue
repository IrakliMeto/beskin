<template>
  <header class="header">
    <div class="container padding header__inner">
      <TheLogo />
      <TheNav class="header__nav" />

      <div class="header__buttons">
        <TheButton type="inline" text="Sign In" />
        <TheButton type="small" text="Register" />
      </div>
    </div>
  </header>
</template>

<script>
import TheLogo from "@/components/TheLogo";
import TheNav from "@/components/TheNav";
import TheButton from "@/components/TheButton";

export default {
  name: "TheHeader",
  components: {
    TheButton,
    TheNav,
    TheLogo,
  },
};
</script>

<style scoped lang="scss">
.header {
  width: 100%;
  padding: 38px 0;
  background-color: #e6f0ff;

  &__inner {
    display: flex;
    align-items: center;
  }

  &__nav {
    margin: 0 64px;

    @media (max-width: 1023px) {
      margin: 0 30px;
    }
  }

  &__buttons {
    margin-left: auto;
    display: flex;
    align-items: center;
  }
}
</style>
