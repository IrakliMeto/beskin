<template>
  <div class="card">
    <img
      class="card__image"
      src="@/assets/images/photos/house.png"
      alt="House Image"
    />

    <div class="card__content">
      <h6 class="card__price">{{ price }}</h6>

      <p class="card__text">{{ text }}</p>

      <div class="card__bottom">
        <div class="card__about">
          <img src="@/assets/images/icons/bed.svg" alt="" /> {{ beds }}
        </div>
        <div class="card__about">
          <img src="@/assets/images/icons/bath.svg" alt="" /> {{ bath }}
        </div>
        <div class="card__about">
          <img src="@/assets/images/icons/fullscreen.svg" alt="" />
          {{ size }}
        </div>
      </div>
    </div>
  </div>
</template>

<script>
export default {
  name: "MediumCard",
  props: {
    price: {
      type: String,
    },
    text: {
      type: String,
    },
    beds: {
      type: String,
    },
    bath: {
      type: String,
    },
    size: {
      type: String,
    },
  },
};
</script>

<style scoped lang="scss">
.card {
  max-width: 350px;
  width: 100%;
  background: #ffffff;
  box-shadow: 0 65px 80px -46px rgba(226, 238, 249, 0.6);
  border-radius: 12px;

  @media (max-width: 1023px) {
    max-width: unset;
  }

  &__image {
    width: 100%;
    height: auto;
    object-fit: cover;
  }

  &__content {
    width: 100%;
    padding: 20px;
  }

  &__price {
    margin-bottom: 8px;
    font-family: "Poppins";
    font-style: normal;
    font-weight: 600;
    font-size: 20px;
    line-height: 20px;
    color: #000339;
  }

  &__text {
    margin-bottom: 21px;
    font-family: "Poppins";
    font-style: normal;
    font-weight: 500;
    font-size: 14px;
    line-height: 21px;
    color: #a3a6ab;
  }

  &__bottom {
    display: flex;
    align-items: center;
    justify-content: space-between;
    gap: 0 10px;
  }

  &__about {
    display: flex;
    align-items: center;
    font-family: "Poppins";
    font-style: normal;
    font-weight: 500;
    font-size: 14px;
    line-height: 14px;

    @media (max-width: 1240px) {
      font-size: 12px;
    }

    img {
      margin-right: 8px;
    }
  }
}
</style>
