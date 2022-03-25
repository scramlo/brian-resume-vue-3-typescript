<script setup lang="ts">
defineProps({
  date: {
    type: String,
    required: false,
    default: "",
  },
  degree: {
    type: String,
    required: false,
    default: "",
  },
  school: {
    type: String,
    required: false,
    default: "",
  },
  location: {
    type: String,
    required: false,
    default: "",
  },
});
</script>
<template>
  <div class="education-group">
    <div class="education-group__date">{{ date }}</div>
    <div class="education-group__degree">{{ degree }}</div>
    <div class="education-group__school">{{ school }}</div>
    <div class="education-group__location">{{ location }}</div>
  </div>
</template>
<style scoped lang="scss">
.education-group {
  display: flex;
  flex-direction: column;
  gap: 1rem;
  &__degree {
    font-weight: bold;
    font-size: 1.25rem;
    text-transform: uppercase;
  }
}
</style>
