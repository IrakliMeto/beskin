<template>
  <div class="banner-container">
    <div class="container banner">
      <div class="banner__box">
        <h5 class="banner__subtitle">Welcome to Besnik Agency</h5>

        <h3 class="banner__title">Discover a place you'll love to live.</h3>

        <p class="banner__text">
          get the best real estate deals first, before they hit the mass market!
          HOT FORECLOSURE DEALS with one simple search
        </p>

        <TheButton type="medium" text="More About Us" />
      </div>
      <img
        src="@/assets/images/photos/banner.png"
        alt="Banner Image"
        class="banner__image"
      />
    </div>
  </div>
</template>

<script>
import TheButton from "@/components/helper/TheButton";
export default {
  name: "TheBanner",
  components: { TheButton },
};
</script>

<style scoped lang="scss">
.banner-container {
  background-color: #e6f0ff;
}

.banner {
  padding: 0 65px 0 165px;
  display: flex;
  align-items: center;
  justify-content: space-between;

  @media (max-width: 1240px) {
    padding: 0 40px 0 70px;
  }

  @media (max-width: 1023px) {
    padding: 0 20px 0 40px;
  }

  @media (max-width: 767px) {
    padding: 0 22px;
  }

  &__box {
    margin-right: 30px;

    @media (max-width: 1240px) {
      padding-bottom: 40px;
    }

    @media (max-width: 767px) {
      margin: 0 auto;
      padding: 30px 0;
      display: flex;
      flex-direction: column;
      align-items: center;
      text-align: center;
    }
  }

  &__image {
    width: auto;
    margin-top: auto;

    @media (max-width: 1240px) {
      max-width: 400px;
    }

    @media (max-width: 767px) {
      display: none;
    }
  }

  &__subtitle {
    margin-bottom: 8px;
    font-family: "Poppins";
    font-style: normal;
    font-weight: 500;
    font-size: 18px;
    line-height: 27px;
    letter-spacing: 0.01em;
    color: #687691;

    @media (max-width: 1023px) {
      font-size: 16px;
      line-height: 24px;
    }
  }

  &__title {
    margin-bottom: 30px;
    font-family: "Poppins";
    font-style: normal;
    font-weight: 700;
    font-size: 64px;
    line-height: 76px;
    color: #000336;

    @media (max-width: 1240px) {
      font-size: 56px;
      line-height: 65px;
    }

    @media (max-width: 1023px) {
      font-size: 34px;
      line-height: 40px;
    }
  }

  &__text {
    margin-bottom: 40px;
    font-family: "Poppins";
    font-style: normal;
    font-weight: 400;
    font-size: 18px;
    line-height: 32px;
    color: #5a6473;

    @media (max-width: 1023px) {
      font-size: 16px;
      line-height: 24px;
    }
  }
}
</style>
