<template>
  <nav class="nav">
    <a class="nav__link nav__link--active" href="#"> Home </a>
    <a class="nav__link" href="#"> Fratures </a>
    <a class="nav__link" href="#"> Service </a>
    <a class="nav__link" href="#"> Listed </a>
    <a class="nav__link" href="#"> Contact </a>
  </nav>
</template>

<script>
export default {
  name: "TheNav",
};
</script>

<style scoped lang="scss">
.nav {
  display: flex;
  gap: 0 30px;

  @media (max-width: 1023px) {
    gap: 0 14px;
  }

  @media (max-width: 767px) {
    justify-content: space-between;
  }

  &__link {
    font-family: "Poppins";
    font-style: normal;
    font-weight: 500;
    font-size: 14px;
    line-height: 21px;
    color: #4f5361;
    transition: 0.2s ease;
    position: relative;

    &:after {
      content: "";
      width: 100%;
      height: 1px;
      background: #09143a;
      transition: 0.2s;
      transform: scaleX(0);
      position: absolute;
      left: 0;
      top: 100%;
    }

    &:hover {
      color: #09143a;

      &:after {
        transform: scaleX(1);
      }
    }

    &--active {
      color: #09143a;
    }
  }
}
</style>
