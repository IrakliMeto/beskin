<template>
  <div class="guide-card">
    <img class="guide-card__icon" :src="image" alt="Image" />
    <h5 class="guide-card__title">{{ text }}</h5>
    <LinkWithArrow />
  </div>
</template>

<script>
import LinkWithArrow from "@/components/helper/LinkWithArrow";
export default {
  name: "GuideCard",
  components: { LinkWithArrow },
  props: {
    text: {
      type: String,
    },
    image: {},
  },
};
</script>

<style scoped lang="scss">
.guide-card {
  display: flex;
  flex-direction: column;
  align-items: center;

  &__icon {
    max-width: 48px;
    width: 100%;
    margin-bottom: 26px;
    object-fit: contain;

    @media (max-width: 767px) {
      margin-bottom: 18px;
    }
  }

  &__title {
    margin-bottom: 10px;
    font-family: "Poppins";
    font-style: normal;
    font-weight: 500;
    font-size: 20px;
    line-height: 22px;
    color: #3b3c45;
    text-transform: capitalize;
    text-align: center;

    @media (max-width: 1240px) {
      font-size: 18px;
    }

    @media (max-width: 767px) {
      margin-bottom: 0;
      font-size: 16px;
      line-height: 16px;
    }
  }
}
</style>
