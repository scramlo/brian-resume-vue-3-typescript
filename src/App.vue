<script setup lang="ts">
import TheHeader from "./components/TheHeader.vue";
import SectionContact from "./components/SectionContact.vue";
</script>
<template>
  <div class="layout">
    <TheHeader />
    <main class="main">
      <section class="main__start">
        <SectionContact />
      </section>
      <section class="main__end"></section>
    </main>
  </div>
</template>

<style lang="scss" scoped>
.main {
  display: grid;
  grid-template-columns: 1fr 2fr;

  &__start {
    background-color: var(--brian-accent);
    padding: 1.5rem;
  }
}
</style>
