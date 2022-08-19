<template>
  <div class="about">
    <h3 class="about__title">How its works?</h3>

    <p class="about__text">
      Everything you need to know when you're looking to buy, rent, or sell -
      all in one place.
    </p>

    <div class="about__cards">
      <GuideCard
        :image="require('@/assets/images/icons/cart.svg')"
        text="Buyer Guides"
      />
      <GuideCard
        text="Renter Guides"
        :image="require('@/assets/images/icons/rent.svg')"
      />
      <GuideCard
        text="Seller Guides"
        :image="require('@/assets/images/icons/home.svg')"
      />
    </div>

    <TheButton type="medium" text="Sell Full Guideliness" />
  </div>
</template>

<script>
import GuideCard from "@/components/cards/GuideCard";
import TheButton from "@/components/helper/TheButton";

export default {
  name: "TheAbout",
  components: {
    TheButton,
    GuideCard,
  },
};
</script>

<style scoped lang="scss">
.about {
  width: 100%;
  display: flex;
  flex-direction: column;
  align-items: center;

  &__title {
    margin-bottom: 20px;
    padding-top: 10px;
    position: relative;
    font-family: "Poppins";
    font-style: normal;
    font-weight: 600;
    font-size: 35px;
    line-height: 35px;
    text-align: center;
    color: #000339;

    @media (max-width: 1240px) {
      font-size: 30px;
      line-height: 36px;
    }

    &::before {
      content: "";
      width: 41px;
      height: 4px;
      position: absolute;
      top: 0;
      left: 50%;
      transform: translateX(-50%);
      background: #000339;
      border-radius: 12px;
    }
  }

  &__text {
    max-width: 459px;
    width: 100%;
    font-family: "Poppins";
    font-style: normal;
    font-weight: 400;
    font-size: 16px;
    line-height: 30px;
    text-align: center;
    color: #5a6473;

    @media (max-width: 1024px) {
      max-width: 380px;
      font-size: 14px;
      line-height: 25px;
    }
  }

  &__cards {
    display: flex;
    justify-content: center;
    gap: 0 140px;
    margin: 70px 0 48px;

    @media (max-width: 1240px) {
      gap: 0 100px;
    }

    @media (max-width: 1240px) {
      gap: 0 70px;
    }

    @media (max-width: 767px) {
      gap: 40px;
      flex-wrap: wrap;
    }
  }
}
</style>
