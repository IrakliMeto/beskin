<template>
  <div class="providers">
    <div class="providers__row-holder">
      <div class="content__row">
        <TheLogo class="content__row-logo" />
        <p class="content__row-text">
          More than 45,000+ companies trust besnik
        </p>
      </div>

      <div class="content__row">
        <div class="content__row-icons">
          <img src="@/assets/images/icons/star.svg" alt="Star Icon" />
          <img src="@/assets/images/icons/star.svg" alt="Star Icon" />
          <img src="@/assets/images/icons/star.svg" alt="Star Icon" />
          <img src="@/assets/images/icons/star.svg" alt="Star Icon" />
          <img src="@/assets/images/icons/star.svg" alt="Star Icon" />
        </div>
        <p class="content__row-text">5 Star Ratings (2k+ Review)</p>
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
        <img src="@/assets/images/icons/amazon.svg" alt="" />
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
export default {
  name: "Provider",
};
</script>

<style scoped lang="scss">
.providers {
  &__row-holder {
    width: 100%;
    display: flex;
    justify-content: space-between;
    align-items: center;
  }

  &__row-logo {
    margin-bottom: 23px;

    @media (max-width: 1024px) {
      margin-bottom: 15px;
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
  }

  &__row-icons {
    margin-bottom: 15px;
    text-align: right;
  }
}
</style>
