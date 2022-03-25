<script setup lang="ts">
defineProps({
  width: {
    type: Number,
    required: false,
    default: 100,
  },
  color: {
    type: String,
    required: false,
    default: "var(--brian-accent)",
  },
});
</script>
<template>
  <svg height="5px" :width="`${width}%`">
    <line
      x1="0"
      y1="0"
      x2="1000"
      y2="0"
      style="stroke-width: 5px"
      :style="{ stroke: color }"
    />
  </svg>
</template>
