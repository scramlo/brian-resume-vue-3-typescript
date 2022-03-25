<script setup lang="ts">
import SectionTitle from "@/components/blocks/SectionTitle.vue";
</script>
<template>
  <section class="section-slotted">
    <SectionTitle>
      <template #title>
        <slot name="title"></slot>
      </template>
    </SectionTitle>
    <slot name="text"></slot>
  </section>
</template>
