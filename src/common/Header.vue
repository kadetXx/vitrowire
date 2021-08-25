<template>
  <header :class="transparent ? 'transparent' : ''">
    <img class="logo" src="@/assets/svg/logo.svg" alt="vitrowire" />
    <nav>
      <ul class="menu">
        <li class="menu__item">
          <router-link
            to="/"
            active-class="menu__link--active"
            class="menu__link"
            >Home</router-link
          >
        </li>

        <li class="menu__item">
          <router-link
            to="/about"
            active-class="menu__link--active"
            class="menu__link"
            >About Us</router-link
          >
        </li>

        <li class="menu__item">
          <router-link
            to="/"
            active-class="menu__link--active"
            class="menu__link"
            >Careers</router-link
          >
        </li>

        <li class="menu__item">
          <router-link
            to="/"
            active-class="menu__link--active"
            class="menu__link"
            >Blog</router-link
          >
        </li>

        <li class="menu__item">
          <router-link
            to="/"
            active-class="menu__link--active"
            class="menu__link"
            >Product</router-link
          >
        </li>

        <span class="menu__indicator" ref="indicator">---</span>
      </ul>
    </nav>
    <button class="header__cta">Contact Us</button>
  </header>
</template>

<script>
export default {
  name: "Header",
  props: {
    transparent: Boolean,
  },

  mounted() {
    const activeMenu = document.querySelector(".menu__link--active");
    const indicator = this.$refs.indicator;

    // get right of am
    // get right of

    const activeMenuRight = activeMenu.offsetLeft + activeMenu.offsetWidth;
    indicator.style.left = activeMenuRight - indicator.offsetWidth + "px";
  },
};
</script>

<style lang="scss" scoped>
header {
  background-color: var(--primary);
  padding: 1.5rem 5%;
  display: flex;
  justify-content: space-between;
  align-items: center;
}

header.transparent {
  background-color: transparent;
}

.header__cta {
  border-color: #fff;
  color: #fff;
}

nav {
  margin-left: auto;
  margin-right: 2.5rem;
}

.menu {
  display: flex;
  align-items: center;
  list-style: none;
  margin: 0;
  padding: 0.7rem 0;
  position: relative;
}

.menu__item {
  margin-left: 2.5rem;
}

.menu__link {
  color: #fff;
  text-decoration: none;
}

.menu__indicator {
  position: absolute;
  bottom: 0;
  color: #ff9100;
  font-weight: bold;
  line-height: 0;
  opacity: 0.8;
  transition: all 0.2s linear;
}
</style>
