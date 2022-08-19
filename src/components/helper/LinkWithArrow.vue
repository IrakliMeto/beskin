<template>
  <div>
    <a class="link" href="#">
      {{ text }} <img src="@/assets/images/icons/right-arrow.svg" alt="" />
    </a>
  </div>
</template>

<script>
export default {
  name: "LinkWithArrow",
  props: {
    text: {
      type: String,
      default: "How to buy",
    },
  },
};
</script>

<style scoped lang="scss">
.link {
  font-family: "Poppins";
  font-style: normal;
  font-weight: 600;
  font-size: 14px;
  line-height: 21px;
  text-align: center;
  color: #0689ff;
  transition: 0.2s ease;

  &:hover {
    color: #1370c5;
  }

  img {
    margin-left: 8px;
  }
}
</style>
