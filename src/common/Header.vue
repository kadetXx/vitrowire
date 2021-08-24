<template>
  <header :class="transparent ? 'transparent' : ''">
    <img class="logo" src="@/assets/svg/logo.svg" alt="vitrowire" />
    <nav>
      <ul class="menu">
        <li class="menu__item">
          <router-link to="/" class="menu__link">Home</router-link>
        </li>

        <li class="menu__item">
          <router-link to="/" class="menu__link">About Us</router-link>
        </li>

        <li class="menu__item">
          <router-link to="/" class="menu__link">Careers</router-link>
        </li>

        <li class="menu__item">
          <router-link to="/" class="menu__link">Blog</router-link>
        </li>

        <li class="menu__item">
          <router-link to="/" class="menu__link">Product</router-link>
        </li>
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
}

.menu__item {
  margin-left: 2.5rem;
}

.menu__link {
  color: #FFF;
  text-decoration: none;
}
</style>
