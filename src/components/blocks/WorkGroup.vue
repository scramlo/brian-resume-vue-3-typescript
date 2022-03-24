<script setup lang="ts">
import { CIcon } from "@coreui/icons-vue";
import { cilLocationPin, cilBriefcase } from "@coreui/icons";
defineProps({
  position: {
    type: String,
    required: false,
    default: "",
  },
  company: {
    type: String,
    required: false,
    default: "",
  },
  location: {
    type: String,
    required: false,
    default: "",
  },
  date: {
    type: String,
    required: false,
    default: "",
  },
  description: {
    type: String,
    required: false,
    default: "",
  },
});
</script>
<template>
  <div class="work-group">
    <div class="meta">
      <div class="meta__position-company">
        <div class="meta__position">{{ position }}</div>
        <div class="meta__company">{{ company }}</div>
      </div>
      <div class="meta__location-date">
        <div class="meta__location">
          <CIcon :icon="cilLocationPin" style="width: 1rem" /> &nbsp;<em>{{
            location
          }}</em>
        </div>
        <div class="meta__date">
          <CIcon :icon="cilBriefcase" style="width: 1rem" /> &nbsp;<em>{{
            date
          }}</em>
        </div>
      </div>
    </div>
    <div class="work-group__description">{{ description }}</div>
  </div>
</template>
<style scoped lang="scss">
.work-group {
  display: grid;
  gap: 1rem;
  margin-bottom: 2rem;

  .meta {
    display: grid;
    grid-template-columns: 1fr 1fr;
    &__position {
      font-weight: bold;
      font-size: 1.25rem;
      text-transform: uppercase;
      display: block;
      margin-bottom: 0.5rem;
    }

    &__location {
      margin-bottom: 0.5rem;
    }
  }

  &__description {
    line-height: 2rem;
  }
}
</style>
