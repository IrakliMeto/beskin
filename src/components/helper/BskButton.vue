<template>
  <button class="button" :class="[`button--${type}`]">{{ text }}</button>
</template>

<script>
export default {
  name: "BskButton",
  props: {
    type: {
      type: String,
      default: "medium",
    },
    text: {
      type: String,
    },
  },
};
</script>

<style scoped lang="scss">
.button {
  padding: 10px 20px;
  display: flex;
  align-items: center;
  font-family: "Poppins";
  font-style: normal;
  font-weight: 500;
  font-size: 14px;
  line-height: 21px;
  text-align: center;
  color: #ffffff;
  outline: none;
  border: none;
  transition: 0.2s ease;
  cursor: pointer;
  text-transform: capitalize;
  background: #0f1b4c;
  border-radius: 12px;

  @media (max-width: 767px) {
    font-size: 13px;
  }

  &:hover {
    background: #253888;
  }

  &--medium {
    height: 50px;
    padding: 10px 25px;
    font-size: 13px;

    @media (max-width: 767px) {
      height: 40px;
      font-size: 12px;
    }
  }

  &--small {
    height: 40px;

    @media (max-width: 767px) {
      height: 34px;
    }
  }

  &--white {
    background: #ffffff;
    color: #002366;

    &:hover {
      background: #f0eded;
    }
  }

  &--inline {
    color: #0f1b4c;
    background-color: transparent;
    border: none;

    &:hover {
      color: #253888;
      background-color: transparent;
    }
  }
}
</style>
