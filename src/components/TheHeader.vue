<script setup lang="ts">
import SvgLine from "@/components/ui/SvgLine.vue";
// const profileImgSrcLqip = `https://res.cloudinary.com/nerd-specs-creative/image/upload/c_fill,dpr_auto,e_blur:100,f_auto,g_north,h_500,q_auto:low/v1648082776/headshotsscramlin-77_dpkljh.jpg`;
const profileImgSrc = `https://res.cloudinary.com/nerd-specs-creative/image/upload/c_fill,dpr_auto,f_auto,g_center,h_1000,q_auto,w_667/v1648082776/headshotsscramlin-77_dpkljh.jpg`;
</script>

<template>
  <header class="header">
    <section class="header__title-wrapper">
      <SvgLine :width="80" />
      <h1 class="title">Brian Scramlin</h1>
      <SvgLine :width="100" />
      <span class="subtitle">Developer + Designer</span>
    </section>
    <section class="header__profile-image-wrapper">
      <img
        class="profile-image"
        :src="profileImgSrc"
        alt="Brian Scramlin"
        height="500"
        width="333.5"
      />
    </section>
    <section class="header__description-wrapper">
      <p class="description">
        “Don't ask what the world needs. Ask what makes you
        <span>come alive</span>… Because what the world needs is people who have
        <span>come alive</span>.” -Howard Thurman
      </p>
    </section>
  </header>
</template>

<style lang="scss" scoped>
.header {
  background-color: var(--brian-dark);
  display: grid;
  grid-template-columns: 1fr 1fr 1fr;
  color: var(--brian-light);

  &__title-wrapper {
    padding: 1.5rem;
    display: flex;
    gap: 1rem;
    justify-content: center;
    flex-direction: column;
    .title {
      text-transform: uppercase;
      font-size: 3rem;
      margin: 0;
      text-shadow: 0px 10px 10px black;
    }

    .subtitle {
      font-size: 2rem;
    }
  }

  &__profile-image-wrapper {
    display: flex;
    justify-content: center;
  }

  &__description-wrapper {
    padding: 1.5rem;
    display: flex;
    align-items: center;

    .description {
      font-size: 1.5rem;
      line-height: 1.5;

      span {
        color: var(--brian-accent);
      }
    }
  }
}
</style>
