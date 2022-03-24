<script setup lang="ts">
import TheHeader from "./components/TheHeader.vue";
import SectionContact from "./components/SectionContact.vue";
import SectionExpertise from "./components/SectionExpertise.vue";
import SectionSkills from "./components/SectionSkills.vue";
import SectionEducation from "./components/SectionEducation.vue";
import SectionWork from "./components/SectionWork.vue";
import SectionMyStory from "./components/SectionMyStory.vue";
</script>
<template>
  <div class="layout">
    <TheHeader />
    <main class="main">
      <section class="main__start">
        <SectionContact />
        <SectionExpertise />
        <SectionSkills />
      </section>
      <section class="main__end">
        <SectionMyStory />

        <SectionWork />
      </section>
    </main>
  </div>
</template>

<style lang="scss" scoped>
.main {
  display: grid;
  grid-template-columns: 1fr 2fr;

  section {
    padding: 0.75rem;
  }

  &__start {
    background-color: var(--brian-accent);
  }
}
</style>
