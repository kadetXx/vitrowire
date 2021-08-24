<template>
  <div id="app">
    <router-view />
  </div>
</template>

<style lang="scss">
@import url("http://fonts.cdnfonts.com/css/monument-extended");

* {
  font-family: "Monument Extended", sans-serif;
  box-sizing: border-box;
  scroll-behavior: smooth;

  --primary: #402a85;
  --primary-100: #45108a;
  --primary-200: #352058;
  --secondary: #43e8e1;
  --tetiary: #ffa98c;
  --black: #130217;
}

#app {
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  text-align: center;
  color: var(--black);
}
</style>
