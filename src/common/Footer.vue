<template>
  <footer>
    <div class="footer">
      <div class="footer__logo-container">
        <img src="@/assets/svg/logo-alt.svg" alt="logo" class="footer__logo" />
        <p class="footer__description">
          We are a tech product and services marketing agency specialized in
          bringing products to the notice and acceptance of the necessary target
          market across Africa,
        </p>
      </div>

      <ul class="nav">
        <h4 class="nav__title">Quick Links</h4>
        <li class="nav__item">
          <a href="#">About Us</a>
        </li>

        <li class="nav__item">
          <a href="#">Blog</a>
        </li>

        <li class="nav__item">
          <a href="#">Partners</a>
        </li>

        <li class="nav__item">
          <a href="#">Careers</a>
        </li>
      </ul>

      <ul class="nav">
        <h4 class="nav__title">Our Services</h4>
        <li class="nav__item">
          <a href="#">Branding</a>
        </li>

        <li class="nav__item">
          <a href="#">Markekting</a>
        </li>

        <li class="nav__item">
          <a href="#">Strategy Consulting</a>
        </li>

        <li class="nav__item">
          <a href="#">Marketing Management</a>
        </li>
      </ul>

      <ul class="nav">
        <h4 class="nav__title">Talk to Us</h4>
        <li class="nav__item">
          <a href="#"
            ><img src="@/assets/svg/pin.svg" alt="location" /> J25B, Road 3,
            VGC, Lagos</a
          >
        </li>

        <li class="nav__item">
          <a target="blank" _ href="https://wa.me/2348135244971"
            ><img src="@/assets/svg/whatsapp.svg" alt="whatsapp" /> +234 813
            5244 971</a
          >
        </li>

        <li target="blank" class="nav__item">
          <a href="https://t.me/2348036339183">
            <img src="@/assets/svg/telegram.svg" alt="telegram" />+234 803 633
            9183</a
          >
        </li>

        <li target="blank" class="nav__item">
          <a href="mailto:hello@vitrowire.com"
            ><img
              src="@/assets/svg/email.svg"
              alt="mail"
            />hello@vitrowire.com</a
          >
        </li>
      </ul>
    </div>
    <div class="copyright">
      <p class="copyright__text">
        Copyright 2021 Vitrowire. All rights reserved.
      </p>
    </div>
  </footer>
</template>

<style lang="scss" scoped>
footer {
  padding: 2rem 5%;
  margin-top: 12%;
}

a {
  text-decoration: none;
  color: unset;
}

.footer {
  display: grid;
  grid-template-columns: 1.2fr repeat(3, 1fr);
  padding: 0 0 1rem;
  align-items: flex-start;
  justify-content: space-between;
  column-gap: 3rem;

  &__logo {
    max-width: 70%;
  }

  &__description {
    opacity: 0.7;
    line-height: 150%;
  }
}

.nav {
  list-style: none;
  padding: 0;
  margin-left: auto;

  &__title {
    color: var(--primary);
    font-weight: normal;
    margin: 0 0 1.8rem;
    font-size: 0.8rem;
  }

  &__item {
    margin-block: 1rem;
    opacity: 0.8;
    font-size: 0.9rem;

    a {
      display: flex;
      align-items: center;
    }

    img {
      width: 16px;
      height: 16px;
      margin-right: 0.7rem;
    }
  }
}

.copyright {
  border-top: 1px solid rgba(#130217, 0.2);
  padding-top: 0.7rem;

  &__text {
    opacity: 0.5;
  }
}
</style>
