<script setup lang="ts"></script>
<template>
  <div class="info-group">
    <div class="info-group__icon">
      <slot name="icon" />
    </div>
    <div class="info-group__info">
      <slot name="title" />
      <slot name="info" />
    </div>
  </div>
</template>
<style scoped lang="scss">
.info-group {
  display: grid;
  grid-template-columns: 30px max-content;
  align-items: center;
  gap: 1.5rem;

  &__info {
    display: flex;
    flex-direction: column;
  }
}
</style>
