<script lang="ts" setup>
import SectionTitle from "@/components/blocks/SectionTitle.vue";
</script>

<template>
  <section>
    <SectionTitle title="Expertise" />
    <div class="expertise">
      <div class="expertise__list">
        <h3 class="expertise__list-title">Daily</h3>
        <div class="expertise__list-content">
          <span
            ><strong>Vue.js:</strong> 2, 3, Composition API, Vuex, Vue Router,
            Vuetify, Buefy</span
          >
          <span><strong>TypeScript:</strong> Types, Interfaces, Enums</span>
          <span>
            <strong>ES6:</strong> Modules, Arrow Functions, Nullish Coalescing,
            Optional Chaining
          </span>
          <span><strong>SASS:</strong> Dart Sass 1.23+, @use, @forward</span>
          <span
            ><strong>Jest / Cypress:</strong> Unit Tests, End to End Tests</span
          >
        </div>
      </div>
      <div class="expertise__list">
        <h3 class="expertise__list-title">Less Often</h3>
        <div class="expertise__list-content">
          <span
            ><strong>PHP: </strong> Laravel, ProcessWire, Moodle, Classes,
            Autoloading
          </span>
          <span
            ><strong>Ruby on Rails:</strong> Model Generation, Templating,
            Controller Logic</span
          >
          <span>
            <strong>JS Frameworks / Tools:</strong> React, Web Components,
            Angular, Ionic, Cordova
          </span>
        </div>
      </div>
    </div>
  </section>
</template>

<style lang="scss" scoped>
.expertise {
  display: grid;
  gap: 1rem;

  &__list {
    display: grid;
    gap: 1rem;
  }

  &__list-content {
    display: grid;
    gap: 1rem;
    border: 2px dashed var(--brian-dark);
    padding: 1rem;
  }

  &__list-title {
    margin: 0;
    text-align: center;
  }
}
</style>
