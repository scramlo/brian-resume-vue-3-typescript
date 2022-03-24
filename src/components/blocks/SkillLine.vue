<script setup lang="ts">
defineProps({
  level: {
    type: Number,
    required: false,
    default: 50,
  },
  skill: {
    type: String,
    required: false,
    default: "",
  },
});
</script>
<template>
  <div class="skill-line">
    <h3 class="skill-line__title">{{ skill }}</h3>
    <svg width="100%" height="25">
      <!-- The Box -->
      <rect
        width="100%"
        height="25"
        style="stroke-width: 3; stroke: rgb(0, 0, 0); fill: none"
      />
      <!-- The Level -->
      <rect
        width="22"
        height="23"
        :x="`${level}%`"
        y="1"
        style="fill: var(--brian-dark)"
      />
    </svg>
  </div>
</template>

<style scoped lang="scss">
.skill-line {
  &__title {
    margin: 0;
  }
}
</style>
