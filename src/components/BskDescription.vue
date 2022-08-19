<template>
  <div class="description">
    <div class="container description__content">
      <div class="description__row">
        <div class="description__card">
          <div class="description__card-holder">
            <StatisticsCard />
          </div>
          <img
            class="description__image"
            src="@/assets/images/photos/building.jpg"
            alt="Building Image"
          />
        </div>
        <div class="description__box">
          <h5 class="description__title">
            You’ve found a neighborhood you love.
          </h5>

          <p class="description__text">
            When you own a home, you’re committing to living in one location for
            a while. In a recent Trulia survey, we found that five out of six
            respondents said finding the right neighborhood
          </p>
        </div>
      </div>

      <div class="description__block">
        <div class="description__col">
          2,500
          <span> Homes For Sale </span>
        </div>
        <div class="description__col">
          5,000+
          <span> Homes Recently Sold </span>
        </div>
        <div class="description__col">
          170+
          <span> Price Reduced </span>
        </div>
      </div>
    </div>
  </div>
</template>

<script>
import StatisticsCard from "@/components/cards/StatisticsCard";
export default {
  name: "BskDescription",
  components: { StatisticsCard },
};
</script>

<style scoped lang="scss">
.description {
  width: 100%;
  background-color: #fff;

  &__row {
    padding: 125px 250px 110px 316px;
    display: flex;
    justify-content: space-between;
    align-items: center;
    gap: 50px;

    @media (max-width: 1439px) {
      padding: 125px 180px 110px 230px;
    }

    @media (max-width: 1240px) {
      padding: 125px 120px 110px 180px;
      gap: 30px;
    }

    @media (max-width: 1024px) {
      flex-direction: column;
      gap: 70px 0;
    }

    @media (max-width: 767px) {
      padding: 60px 20px;
    }
  }

  &__box {
    max-width: 309px;
    width: 100%;

    @media (max-width: 1240px) {
      max-width: 270px;
    }

    @media (max-width: 1024px) {
      max-width: unset;
      text-align: center;
    }
  }

  &__card {
    position: relative;
  }

  &__card-holder {
    position: absolute;
    top: 0;
    left: -120px;

    @media (max-width: 767px) {
      display: block;
      position: unset;
    }
  }

  &__image {
    width: 400px;
    max-height: 460px;
    border-radius: 12px;

    @media (max-width: 1240px) {
      max-width: 340px;
    }

    @media (max-width: 1024px) {
      max-width: 400px;
    }

    @media (max-width: 767px) {
      display: none;
    }
  }

  &__title {
    padding-top: 10px;
    margin-bottom: 20px;
    position: relative;
    font-family: "Poppins";
    font-style: normal;
    font-weight: 600;
    font-size: 35px;
    line-height: 45px;
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
      background: #000339;
      border-radius: 12px;
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
      line-height: 24px;
    }
  }

  &__block {
    padding: 0 196px 103px 259px;
    display: flex;
    align-items: center;
    justify-content: space-between;
    gap: 30px;

    @media (max-width: 1439px) {
      padding: 0 142px 103px 192px;
    }

    @media (max-width: 1240px) {
      padding: 0 100px 103px 142px;
    }

    @media (max-width: 1024px) {
      padding: 0 70px 60px 100px;
    }

    @media (max-width: 767px) {
      padding: 0 30px 60px;
      justify-content: center;
      flex-wrap: wrap;
    }
  }

  &__col {
    display: flex;
    flex-direction: column;
    font-family: "Poppins";
    font-style: normal;
    font-weight: 600;
    font-size: 64px;
    line-height: 64px;
    color: #000000;

    @media (max-width: 1240px) {
      font-size: 50px;
      line-height: 50px;
    }

    @media (max-width: 1024px) {
      font-size: 36px;
      line-height: 30px;
    }

    span {
      margin-top: 22px;
      font-weight: 500;
      font-size: 18px;
      line-height: 27px;
      color: #7b8087;

      @media (max-width: 1024px) {
        margin-top: 15px;
        font-size: 15px;
        line-height: 20px;
      }
    }
  }
}
</style>
