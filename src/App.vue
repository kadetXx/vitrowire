<template>
  <div id="app">
    <router-view />
  </div>
</template>

<style lang="scss">
@import url("https://fonts.cdnfonts.com/css/monument-extended");
@import url("https://fonts.googleapis.com/css2?family=DM+Sans:wght@400;500;700&display=swap");

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

body {
  margin: 0;
}

#app {
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  color: var(--black);
}

p,
a,
span,
small,
button {
  font-family: "DM Sans", sans-serif;
}

button {
  padding: 0.8rem 2rem;
  font-size: 0.9rem;
  outline: none;
  background-color: transparent;
  border-radius: 10px;
  border: 1px solid;
  transition: all 0.2s;

  &:hover {
    opacity: 0.8;
    transform: scale(0.9);
  }
}
</style>
