<template>
  <header class="header">
    <div class="container padding header__inner">
      <TheLogo />
      <TheNav class="header__nav header__nav--desktop" />

      <div class="header__buttons">
        <TheButton type="inline" text="Sign In" />
        <TheButton type="small" text="Register" />
      </div>

      <TheNav class="header__nav header__nav--mobile" />
    </div>
  </header>
</template>

<script>
import TheLogo from "@/components/helper/TheLogo";
import TheNav from "@/components/navigation/TheNav";
import TheButton from "@/components/helper/TheButton";

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

  @media (max-width: 767px) {
    padding: 20px 0;
    border-bottom: 2px solid #000339;
  }

  &__inner {
    display: flex;
    align-items: center;

    @media (max-width: 767px) {
      flex-wrap: wrap;
    }
  }

  &__nav {
    margin: 0 64px;

    @media (max-width: 1023px) {
      margin: 0 30px;
    }

    @media (max-width: 767px) {
      margin: 20px auto 0;
    }

    &--desktop {
      display: none;

      @media (min-width: 768px) {
        display: flex;
      }
    }

    &--mobile {
      display: flex;

      @media (min-width: 768px) {
        display: none;
      }
    }
  }

  &__buttons {
    margin-left: auto;
    display: flex;
    align-items: center;
  }
}
</style>
