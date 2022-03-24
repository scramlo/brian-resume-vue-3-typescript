<script setup lang="ts">
defineProps({
  title: {
    type: String,
    required: false,
    default: "",
  },
});
</script>
<template>
  <h2 class="section-title">
    {{ title }}
    <slot name="title"></slot>
  </h2>
</template>

<style scoped lang="scss">
.section-title {
  text-transform: uppercase;
  padding: 1rem;
  border-top: 2px solid var(--brian-dark);
  border-right: 2px solid var(--brian-dark);
  border-bottom: 2px solid var(--brian-dark);
}
</style>
