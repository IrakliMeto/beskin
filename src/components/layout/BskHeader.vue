<template>
  <header class="header">
    <div class="container padding header__inner">
      <div class="header__holder">
        <BskLogo />
        <BskNav class="header__nav header__nav--desktop" />

        <div class="header__buttons">
          <BskButton type="inline" text="Sign In" />
          <BskButton type="small" text="Register" />
        </div>
      </div>

      <BskNav class="header__nav header__nav--mobile" />
    </div>
  </header>
</template>

<script>
import BskLogo from "@/components/helper/BskLogo";
import BskNav from "@/components/navigation/BskNav";
import BskButton from "@/components/helper/BskButton";

export default {
  name: "BskHeader",
  components: {
    BskButton,
    BskNav,
    BskLogo,
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
      flex-direction: column;
    }
  }

  &__holder {
    width: 100%;
    display: flex;
    justify-content: space-between;
    align-items: center;
  }

  &__nav {
    margin: 0 64px;

    @media (max-width: 1023px) {
      margin: 0 30px;
    }

    @media (max-width: 767px) {
      width: 100%;
      margin: 10px 0 0;
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
