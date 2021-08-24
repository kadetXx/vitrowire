<template>
  <div id="hero">
    <Header :transparent="true" />
    <div class="hero__wrapper">
      <div class="hero__section">
        <h1 class="hero__title">
          Catapult your blockchain project using digital and traditional means
        </h1>
        <p class="hero__subtitle">
          Got a blockchain solution? <br />
          Wanna get Africa stongly involved? <br />
          Let’s whisper into the right ears
        </p>
        <div class="hero__cta-wrapper">
          <button>Request a call</button>
          <button>Learn more</button>
        </div>
        <div class="hero__socials">
          <a class="hero__link" href="#">Fb</a>
          <a class="hero__link" href="#">Tw</a>
          <a class="hero__link" href="#">Ln</a>
          <a class="hero__link" href="#">Ig</a>
        </div>
      </div>

      <div class="hero__section">
        <img
          class="hero__image"
          src="@/assets/svg/hero-image.svg"
          alt="hero image"
        />
      </div>
    </div>
  </div>
</template>

<script>
import Header from "@/common/Header.vue";
export default {
  name: "Hero",
  components: {
    Header,
  },
};
</script>

<style lang="scss" scoped>
#hero {
  display: flex;
  flex-direction: column;
  min-height: 100vh;
  background: linear-gradient(
    243.3deg,
    #402a85 -8.71%,
    #402a85 -5.14%,
    #352058 43.12%,
    #201e4c 168.23%
  );
}

.hero__wrapper {
  display: grid;
  grid-template-columns: 1.1fr 0.9fr;
  column-gap: 2rem;
  flex-grow: 1;
  padding: 3.5rem 5% 2rem;
}

.hero__section:first-child {
  display: flex;
  flex-direction: column;
  align-items: flex-start;
  justify-content: flex-start;
  color: #fff;

  .hero__title {
    font-size: 2.8rem;
    font-weight: 500;
    margin-bottom: 0;
    /* line-height: 130%; */
  }

  .hero__subtitle {
    font-size: 1.1rem;
    line-height: 150%;
    margin: 2rem 0;
  }

  .hero__cta-wrapper {
    display: flex;
    align-items: center;

    button {
      padding: 0.9rem 2.7rem;
      font-size: 1rem;
    }

    button:first-child {
      margin-right: 1rem;
      background-color: var(--secondary);
      color: var(--primary-100);
      border-color: var(--secondary);
    }

    button:last-child {
      margin-right: 1rem;
      color: var(--secondary);
      border-color: var(--secondary);
    }
  }

  .hero__socials {
    margin-top: 2rem;
    display: flex;
    align-items: flex-end;

    .hero__link {
      margin-right: 2.5rem;
      color: var(--tetiary);
      text-decoration-color: var(--tetiary);
    }
  }
}

.hero__section:last-child {
  display: flex;
  align-items: center;
  justify-content: flex-start;

  .hero__image {
    max-height: 100%;
    max-width: 90%;
  }
}
</style>
