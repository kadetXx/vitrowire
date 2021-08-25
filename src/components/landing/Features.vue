<template>
  <div id="details">
    <div class="cta">
      <span class="cta__pretitle">
        - AFRICA’S FIRST HIGH-TECH MARKETING AGENCY -
      </span>
      <h2 class="cta__title">
        Let’s help you scale your <br />
        tech product or service
      </h2>
      <p class="cta__subtitle">
        Looking to see your tech solution across Africa? Let’s tell the
        continent; <br />
        or maybe just your preferred village
      </p>
      <a href="#"><button class="cta__button">Talk to us</button></a>
    </div>

    <div class="features">
      <div class="features__box">
        <img
          src="@/assets/svg/icon-one.svg"
          alt="icon"
          class="features__icon"
        />
        <h3 class="features__title">Marketing Advisory</h3>
        <p class="features__subtitle">
          Avoid wasting your marketing budget. Make the best choices for your
          blockchain project launch, token pre-sale, IEO, ICO, brand building,
          across Africa
        </p>
        <a href="#" class="features__link"
          >Request a call <i class="material-icons">chevron_right</i></a
        >
      </div>

      <div class="features__box">
        <img
          src="@/assets/svg/icon-two.svg"
          alt="icon"
          class="features__icon"
        />
        <h3 class="features__title">Token Marketing</h3>
        <p class="features__subtitle">
          Launching or running an IEO or ICO? Are you looking to build a solid
          digital presence across Africa? Let’s have a chat.
        </p>
        <a href="#" class="features__link"
          >Request a call <i class="material-icons">chevron_right</i></a
        >
      </div>

      <div class="features__box">
        <img
          src="@/assets/svg/icon-three.svg"
          alt="icon"
          class="features__icon"
        />
        <h3 class="features__title">Brand Marketing Strategy</h3>
        <p class="features__subtitle">
          Pemetrate, maintain, improve, and grow your blockchain project
          community across Africa. Get the best-tailored blockchain brand
          strategy and marketing.
        </p>
        <a href="#" class="features__link"
          >Request a call <i class="material-icons">chevron_right</i></a
        >
      </div>
    </div>
  </div>
</template>

<script>
export default {
  name: "Features",
};
</script>

<style lang="scss" scoped>
#details {
  padding: 3rem 5% 0;
}

a {
  text-decoration: none;
  color: unset;
}

.cta {
  text-align: center;

  &__pretitle {
    color: var(--black);
    opacity: 0.6;
    font-size: 0.9rem;
    font-weight: normal;
    font-family: "Monument Extended", sans-serif;
  }

  &__subtitle {
    color: var(--black);
    opacity: 0.8;
    font-size: 1.1rem;
    margin-top: 0;
  }

  &__title {
    font-weight: 500;
    font-size: 2.5rem;
  }

  &__button {
    margin-top: 1rem;
    padding-left: 3.5rem;
    padding-right: 3.5rem;
    background-color: var(--primary);
    color: #ffffff;
    border-color: var(--primary);
    font-size: 1rem;
  }
}

.features {
  display: grid;
  grid-template-columns: repeat(3, 1fr);
  column-gap: 5%;
  padding: 10% 0 8%;
  color: var(--black);

  &__subtitle {
    opacity: 0.7;
    line-height: 150%;
  }

  &__link {
    color: var(--secondary);
    text-decoration: none;
    display: flex;
    align-items: center;

    i {
      margin-left: 0.1rem;
    }
  }
}
</style>
