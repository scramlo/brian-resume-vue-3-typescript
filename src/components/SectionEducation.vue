<script setup lang="ts">
import SectionTitle from "@/components/blocks/SectionTitle.vue";
import EducationGroup from "@/components/blocks/EducationGroup.vue";
</script>
<template>
  <section class="education">
    <SectionTitle title="Education" />
    <div class="education__list">
      <EducationGroup
        date="2005 - 2009"
        degree="Bachelor of Arts"
        school="Indiana Wesleyan University"
        location="USA ( Marion, IN )"
      />
      <EducationGroup
        date="2020 - Present"
        degree="Master of Arts"
        school="Portland Seminary / Wesley Seminary"
        location="USA ( Portland, OR ), USA ( Marion, IN )"
      />
      <EducationGroup
        date="2022"
        degree="W3C Web Accessibility"
        school="World Wide Web Consortium (W3C)"
        location="Online"
      />
    </div>
  </section>
</template>

<style scoped lang="scss">
.education {
  &__list {
    display: grid;
    grid-template-columns: 1fr 1fr 1fr;
  }
}
</style>
