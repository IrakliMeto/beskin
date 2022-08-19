<template>
  <div class="statistic-card">
    <div class="statistic-card__head">
      <h4 class="statistic-card__title">40,000+</h4>
      <p class="statistic-card__text">
        By avarage for 2 bedroom apments in San Francisco, CA
      </p>
    </div>
    <div class="statistic-card__bottom">
      <div class="statistic-card__icons">
        <img
          src="@/assets/images/icons/profile.png"
          alt="Profile Icon"
          class="statistic-card__icon"
        />
        <img
          src="@/assets/images/icons/profile.png"
          alt="Profile Icon"
          class="statistic-card__icon"
        />
      </div>

      <div class="statistic-card__icons">
        <img
          src="@/assets/images/icons/profile.png"
          alt="Profile Icon"
          class="statistic-card__icon"
        />
        <img
          src="@/assets/images/icons/profile.png"
          alt="Profile Icon"
          class="statistic-card__icon"
        />
        <img
          src="@/assets/images/icons/profile.png"
          alt="Profile Icon"
          class="statistic-card__icon"
        />
        <img
          src="@/assets/images/icons/profile.png"
          alt="Profile Icon"
          class="statistic-card__icon"
        />
      </div>

      <div class="statistic-card__icons">
        <img
          src="@/assets/images/icons/profile.png"
          alt="Profile Icon"
          class="statistic-card__icon"
        />
        <img
          src="@/assets/images/icons/profile.png"
          alt="Profile Icon"
          class="statistic-card__icon"
        />
        <img
          src="@/assets/images/icons/profile.png"
          alt="Profile Icon"
          class="statistic-card__icon"
        />
      </div>

      <div class="statistic-card__icons">
        <img
          src="@/assets/images/icons/profile.png"
          alt="Profile Icon"
          class="statistic-card__icon"
        />
        <img
          src="@/assets/images/icons/profile.png"
          alt="Profile Icon"
          class="statistic-card__icon"
        />
        <img
          src="@/assets/images/icons/profile.png"
          alt="Profile Icon"
          class="statistic-card__icon"
        />
        <img
          src="@/assets/images/icons/profile.png"
          alt="Profile Icon"
          class="statistic-card__icon"
        />
      </div>

      <div class="statistic-card__icons">
        <img
          src="@/assets/images/icons/profile.png"
          alt="Profile Icon"
          class="statistic-card__icon"
        />
        <img
          src="@/assets/images/icons/profile.png"
          alt="Profile Icon"
          class="statistic-card__icon"
        />
      </div>

      <div class="statistic-card__icons">
        <img
          src="@/assets/images/icons/profile.png"
          alt="Profile Icon"
          class="statistic-card__icon"
        />
        <img
          src="@/assets/images/icons/profile.png"
          alt="Profile Icon"
          class="statistic-card__icon"
        />
      </div>

      <div class="statistic-card__icons">
        <img
          src="@/assets/images/icons/profile.png"
          alt="Profile Icon"
          class="statistic-card__icon"
        />
        <img
          src="@/assets/images/icons/profile.png"
          alt="Profile Icon"
          class="statistic-card__icon"
        />
      </div>
    </div>
  </div>
</template>

<script>
export default {
  name: "StatisticsCard",
};
</script>

<style scoped lang="scss">
.statistic-card {
  width: 240px;
  padding: 45px 22px 40px;
  background: #ffffff;
  box-shadow: 90px 85px 100px rgba(0, 0, 0, 0.06);
  border-radius: 0px 0px 12px 12px;

  &__head {
    padding-bottom: 25px;
    border-bottom: 1px solid #e9e9e9;
  }

  &__title {
    margin-bottom: 8px;
    position: relative;
    font-family: "Poppins";
    font-style: normal;
    font-weight: 700;
    font-size: 26px;
    line-height: 26px;
    letter-spacing: 0.01em;
    color: #000339;

    &:after {
      content: "";
      width: 25px;
      height: 16px;
      position: absolute;
      right: 0;
      top: 50%;
      transform: translateY(-50%);
      background-image: url("@/assets/images/icons/green-arrow.svg");
    }
  }

  &__text {
    font-family: "Poppins";
    font-style: normal;
    font-weight: 400;
    font-size: 12px;
    line-height: 18px;
    color: #a7a7a7;
  }

  &__bottom {
    padding-top: 25px;
    display: flex;
    flex-wrap: wrap;
    gap: 16px 18px;
  }

  &__icons {
    height: 16px;
  }

  &__icon {
    width: 16px;
    margin-left: -3px;
    object-fit: contain;
    border-radius: 50%;
    border: 1px solid grey;
  }
}
</style>
