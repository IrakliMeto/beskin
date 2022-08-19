<template>
  <div class="cards-container">
    <div class="container padding cards-container__inner">
      <div class="cards-container__box">
        <div class="cards-container__text-holder">
          <h5 class="cards-container__title">Featured Properties</h5>
          <p class="cards-container__text">
            Everything you need to know when you're looking
          </p>
        </div>

        <LinkWithArrow
          text="View All Properties"
          class="cards-container__link"
        />
      </div>
      <div class="cards-holder">
        <PropertyCard
          v-for="index in 3"
          :key="index"
          price="$35000"
          text="8502 Preston Rd. Inglewood, Maine 98280"
          beds="5 Beds"
          bath="2 Bath"
          size="2000 Sqft"
          :image="require('@/assets/images/photos/house.png')"
        />
      </div>
    </div>
  </div>
</template>

<script>
import LinkWithArrow from "@/components/helper/LinkWithArrow";
import PropertyCard from "@/components/cards/PropertyCard";

export default {
  name: "CardsContainer",
  components: {
    LinkWithArrow,
    PropertyCard,
  },
};
</script>

<style scoped lang="scss">
.cards-container {
  width: 100%;
  padding: 110px 0;
  background: #f5fafe;

  @media (max-width: 767px) {
    padding: 60px 0;
  }

  &__box {
    width: 100%;
    display: flex;
    justify-content: space-between;
    align-items: flex-end;

    @media (max-width: 767px) {
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
    color: #000339;

    @media (max-width: 1240px) {
      font-size: 30px;
      line-height: 36px;
    }
  }

  &__text {
    font-family: "Poppins";
    font-style: normal;
    font-weight: 400;
    font-size: 16px;
    line-height: 30px;
    color: #5a6473;

    @media (max-width: 1024px) {
      font-size: 14px;
      line-height: 25px;
    }

    @media (max-width: 767px) {
      margin-bottom: 10px;
      line-height: 20px;
    }
  }

  &__link {
    &::v-deep {
      a {
        font-size: 18px;

        @media (max-width: 1240px) {
          font-size: 16px;
        }
      }
    }
  }
}

.cards-holder {
  margin-top: 70px;
  display: grid;
  grid-template-columns: repeat(3, 1fr);
  gap: 30px;

  @media (max-width: 1439px) {
    gap: 20px;
  }

  @media (max-width: 1023px) {
    gap: 30px;
    grid-template-columns: repeat(2, 1fr);
  }

  @media (max-width: 767px) {
    grid-template-columns: repeat(1, 1fr);
  }
}
</style>
