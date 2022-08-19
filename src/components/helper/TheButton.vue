<template>
  <button class="button" :class="[`button--${type}`]">{{ text }}</button>
</template>

<script>
export default {
  name: "TheButton",
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

  &:hover {
    background: #253888;
  }

  &--medium {
    height: 50px;
    padding: 10px 25px;
    font-size: 13px;
  }

  &--small {
    height: 40px;
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
