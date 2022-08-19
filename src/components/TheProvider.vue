<template>
  <div class="providers">
    <div class="providers__row-holder">
      <div class="providers__row">
        <TheLogo class="providers__row-logo" />
        <p class="providers__row-text">
          More than 45,000+ companies trust besnik
        </p>
      </div>

      <div class="providers__row">
        <div class="providers__row-icons">
          <img
            v-for="star in 5"
            :key="star"
            src="@/assets/images/icons/star.svg"
            alt="Star Icon"
          />
        </div>
        <p class="providers__row-text providers__row-text--mobile">
          5 Star Ratings (2k+ Review)
        </p>
      </div>
    </div>

    <div class="providers__logo-holder">
      <div class="providers__logo">
        <img src="@/assets/images/icons/undies.svg" alt="" />
      </div>
      <div class="providers__logo">
        <img src="@/assets/images/icons/slack.svg" alt="" />
      </div>
      <div class="providers__logo">
        <img src="@/assets/images/icons/commerce.svg" alt="" />
      </div>
      <div class="providers__logo">
        <img src="@/assets/images/icons/commerce.svg" alt="" />
      </div>
      <div class="providers__logo">
        <img src="@/assets/images/icons/sitepoint.svg" alt="" />
      </div>
    </div>
  </div>
</template>

<script>
import TheLogo from "@/components/helper/TheLogo";

export default {
  name: "TheProvider",
  components: {
    TheLogo,
  },
};
</script>

<style scoped lang="scss">
.providers {
  &__row-holder {
    width: 100%;
    display: flex;
    justify-content: space-between;
    align-items: center;

    @media (max-width: 767px) {
      gap: 0 20px;
    }
  }

  &__row-logo {
    margin-bottom: 23px;

    @media (max-width: 1024px) {
      margin-bottom: 15px;
    }

    @media (max-width: 767px) {
      margin-bottom: 10px;
    }
  }

  &__row-text {
    font-family: "Poppins";
    font-style: normal;
    font-weight: 500;
    font-size: 16px;
    line-height: 20px;
    color: #7d8589;

    @media (max-width: 1024px) {
      font-size: 14px;
    }

    @media (max-width: 767px) {
      &--mobile {
        text-align: right;
      }
    }
  }

  &__row-icons {
    margin-bottom: 15px;
    text-align: right;

    @media (max-width: 767px) {
      margin-bottom: 10px;
    }
  }

  &__logo-holder {
    margin: 102px 0;
    display: grid;
    grid-template-columns: repeat(5, 1fr);
    gap: 0 20px;

    @media (max-width: 767px) {
      margin: 60px 0;
      grid-template-columns: repeat(3, 1fr);
      gap: 10px 20px;
    }
  }

  &__logo {
    min-height: 28px;
    display: flex;
    align-items: center;
    justify-content: center;

    @media (max-width: 1240px) {
      img {
        width: 80%;
      }

      @media (max-width: 767px) {
        img {
          width: 100%;
        }
      }
    }
  }
}
</style>
