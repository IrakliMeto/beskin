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

  &__link {
    font-family: "Poppins";
    font-style: normal;
    font-weight: 500;
    font-size: 14px;
    line-height: 21px;
    color: #4f5361;
    transition: 0.2s ease;

    &:hover {
      color: #09143a;
    }

    &--active {
      color: #09143a;
    }
  }
}
</style>
