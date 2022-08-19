<template>
  <div class="padding properties-holder">
    <div class="properties">
      <div class="properties__box">
        <h5 class="properties__title">Featured Properties</h5>
        <p class="properties__text">
          Everything you need to know when you're looking
        </p>
        <TheButton type="white" text="Get Started Now" />
      </div>
      <div class="properties__image-holder">
        <img src="@/assets/images/photos/mobile-image.svg" alt="" />
      </div>
    </div>
  </div>
</template>

<script>
import TheButton from "@/components/helper/TheButton";
export default {
  name: "PropertiesBlock",
  components: { TheButton },
};
</script>

<style scoped lang="scss">
.properties {
  max-width: 1100px;
  height: 380px;
  margin: 0 auto;
  display: flex;
  align-items: center;
  background: #063183;
  border-radius: 20px;

  @media (max-width: 1439px) {
    height: 340px;
  }

  @media (max-width: 1240px) {
    height: 329px;
  }

  @media (max-width: 767px) {
    height: unset;
    border-radius: 0;
  }

  &-holder {
    @media (max-width: 767px) {
      padding: 0;
    }
  }

  &__box {
    padding: 20px 0 20px 80px;
    margin-right: 40px;

    @media (max-width: 1439px) {
      padding: 20px 0 20px 50px;
    }

    @media (max-width: 767px) {
      padding: 40px 20px;
      margin: 0 auto;
      display: flex;
      flex-direction: column;
      align-items: center;
      text-align: center;
    }
  }

  &__title {
    margin-bottom: 15px;
    font-family: "Poppins";
    font-style: normal;
    font-weight: 600;
    font-size: 35px;
    line-height: 35px;
    color: #ffffff;

    @media (max-width: 1240px) {
      font-size: 30px;
      line-height: 36px;
    }
  }

  &__text {
    margin-bottom: 20px;
    font-family: "Poppins";
    font-style: normal;
    font-weight: 400;
    font-size: 16px;
    line-height: 30px;
    color: #ffffff;
    opacity: 0.75;

    @media (max-width: 1240px) {
      font-size: 14px;
      line-height: 24px;
    }

    @media (max-width: 767px) {
      margin-bottom: 40px;
    }
  }

  &__image-holder {
    height: 100%;
    width: 521px;
    margin-left: auto;
    position: relative;

    @media (max-width: 1439px) {
      width: 470px;
    }

    @media (max-width: 767px) {
      display: none;
    }

    img {
      height: calc(100% + 30px);
      width: 100%;
      position: absolute;
      bottom: 0;
    }
  }
}
</style>
