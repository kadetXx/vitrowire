<template>
  <div class="brands">
    <h3 class="brands__title">More than 1000 companies trust Vitrowire</h3>

    <div class="brands__images">
      <img class="brands__image" src="@/assets/svg/cowrywise.svg" alt="" />
      <img class="brands__image" src="@/assets/svg/paystack.svg" alt="" />
      <img class="brands__image" src="@/assets/svg/paypal.svg" alt="" />
      <img class="brands__image" src="@/assets/svg/zenith.svg" alt="" />
      <img class="brands__image" src="@/assets/svg/kuda.svg" alt="" />
      <img class="brands__image" src="@/assets/svg/gtbank.svg" alt="" />
    </div>
  </div>
</template>

<script>
export default {
  name: "Brands",
};
</script>

<style lang="scss" scoped>
.brands {
  padding: 6rem 5%;
  text-align: center;
}

.brands__title {
  font-weight: 500;
}

.brands__images {
  display: grid;
  grid-auto-flow: column;
  align-items: center;
  justify-content: space-between;
  margin-top: 2rem;
  padding: 0 5%;
}

.brands__image {
  max-width: 90%;
}
</style>
