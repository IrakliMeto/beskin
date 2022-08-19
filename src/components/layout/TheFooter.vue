<template>
  <footer class="footer">
    <div class="container padding footer__inner">
      <div class="footer__item-holder">
        <div class="footer__item">
          <h5 class="footer__item-title">Product</h5>
          <a href="" class="footer__link">Listing</a>
          <a href="" class="footer__link">Property</a>
          <a href="" class="footer__link">Agents</a>
          <a href="" class="footer__link">Blog</a>
        </div>
        <div class="footer__item">
          <h5 class="footer__item-title">Resources</h5>
          <a href="" class="footer__link">Our Homes</a>
          <a href="" class="footer__link">Member Stories</a>
          <a href="" class="footer__link">Video</a>
          <a href="" class="footer__link">Free trial</a>
        </div>
        <div class="footer__item">
          <h5 class="footer__item-title">Company</h5>
          <a href="" class="footer__link">Patnerships</a>
          <a href="" class="footer__link">Terms of use</a>
          <a href="" class="footer__link">Privacy</a>
          <a href="" class="footer__link">Sitemap</a>
        </div>
        <div class="footer__item">
          <h5 class="footer__item-title">Get in touch</h5>
          <p class="footer__item-text">
            You’ll find your next home, in any style you prefer.
          </p>

          <div class="footer__icon-holder">
            <a
              class="footer__icon"
              target="_blank"
              href="https://www.facebook.com/"
            >
              <img src="@/assets/images/icons/fb.svg" alt="FB Icon" />
            </a>
            <a class="footer__icon" target="_blank" href="https://twitter.com/">
              <img src="@/assets/images/icons/twitter.svg" alt="Twitter Icon" />
            </a>
            <a
              class="footer__icon"
              target="_blank"
              href="https://www.linkedin.com/"
            >
              <img
                src="@/assets/images/icons/linkedin.svg"
                alt="Linkedin Icon"
              />
            </a>
          </div>
        </div>
      </div>

      <div class="footer__bottom">
        <TheLogo />
        <p class="footer__text">Copyright 2020.com, All rights reserved.</p>
      </div>
    </div>
  </footer>
</template>

<script>
import TheLogo from "@/components/helper/TheLogo";

export default {
  name: "TheFooter",
  components: {
    TheLogo,
  },
};
</script>

<style scoped lang="scss">
.footer {
  width: 100%;
  padding: 105px 0 58px;
  background-color: #fff;

  @media (max-width: 767px) {
    padding: 60px 0;
  }

  &__item-holder {
    display: flex;
    justify-content: space-between;
    gap: 0 20px;

    @media (max-width: 767px) {
      gap: 40px 25px;
      flex-wrap: wrap;
    }
  }

  &__item {
    display: flex;
    flex-direction: column;

    @media (max-width: 767px) {
      &:last-child {
        display: none;
      }
    }
  }

  &__item-title {
    margin-bottom: 42px;
    font-family: "Lato";
    font-style: normal;
    font-weight: 700;
    font-size: 20px;
    line-height: 24px;
    color: #1c1c1d;

    @media (max-width: 1023px) {
      margin-bottom: 30px;
      font-size: 18px;
    }

    @media (max-width: 767px) {
      margin-bottom: 20px;
    }
  }

  &__link {
    margin-bottom: 18px;
    font-family: "Poppins";
    font-style: normal;
    font-weight: 400;
    font-size: 16px;
    line-height: 24px;
    color: #7a7a7e;
    transition: 0.2s ease;

    @media (max-width: 1023px) {
      font-size: 14px;
      line-height: 20px;
    }

    @media (max-width: 767px) {
      margin-bottom: 10px;
    }

    &:hover {
      color: #323235;
    }

    &:last-child {
      margin-bottom: 0;
    }
  }

  &__item-text {
    max-width: 257px;
    margin-bottom: 40px;
    font-family: "Poppins";
    font-style: normal;
    font-weight: 400;
    font-size: 16px;
    line-height: 28px;
    color: #7a7a7e;

    @media (max-width: 1023px) {
      font-size: 14px;
      line-height: 24px;
    }
  }

  &__bottom {
    margin-top: 74px;
    display: flex;
    justify-content: space-between;
    align-items: center;

    @media (max-width: 767px) {
      gap: 10px 0;
      flex-direction: column;
    }
  }

  &__text {
    font-family: "Poppins";
    font-style: normal;
    font-weight: 400;
    font-size: 14px;
    line-height: 21px;
    color: #c2c2c2;

    @media (max-width: 1023px) {
      font-size: 12px;
    }
  }

  &__icon-holder {
    display: flex;
    gap: 0 16px;
  }

  &__icon {
    width: 28px;
    height: 28px;
    text-align: center;
    background: #f9f9f9;
    border-radius: 6px;
  }
}
</style>
