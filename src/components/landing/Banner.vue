<template>
  <div class="banner">
    <div class="banner__image-container">
      <img
        class="banner__image"
        src="@/assets/svg/banner-img.svg"
        alt="banner image"
      />
    </div>

    <div class="banner__details">
      <h3 class="banner__title">
        Growing your tech <br />
        business of the future, <br />
        today.
      </h3>
      <p class="banner__subtitle">
        Building a futuristic tech company? Worry about building. we’ll talk
        your work. <br />
        Let’s get the world ready for you!
      </p>

      <a href="#">
        <button class="banner__button">Request a call</button>
      </a>
    </div>
  </div>
</template>

<script>
export default {
  name: "Banner",
};
</script>

<style lang="scss" scoped>
.banner {
  margin: 0 5% 3rem;
  background-color: var(--primary-200);
  border-radius: 20px;
  padding: 3.5rem 10%;
  display: flex;
  justify-content: space-between;
  align-items: center;
}

.banner__image-container {
  padding: 1rem;
  margin-right: 3rem;
}

.banner__image {
  max-width: 90%;
}

.banner__details {
  color: #fff;
}

.banner__title {
  font-size: 2rem;
  font-weight: normal;
  margin: 0;
}

.banner__subtitle {
  line-height: 150%;
  margin: 1.5rem 0;
  opacity: 0.8;
}

.banner__button {
  background-color: #fff;
  border-color: #fff;
  color: var(--primary);
  padding: 0.8rem 3rem;
  font-weight: 500;
}
</style>
