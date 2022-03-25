<script lang="ts" setup>
import SectionTitle from "@/components/blocks/SectionTitle.vue";
import SkillLine from "@/components/blocks/SkillLine.vue";
</script>

<template>
  <section>
    <SectionTitle title="Various Skills" />
    <div class="skill-list">
      <SkillLine :level="75" skill="UX Design" />
      <SkillLine :level="90" skill="Speaking / Writing" />
      <SkillLine :level="60" skill="Jira / Ticketing" />
      <SkillLine :level="80" skill="Motion Graphics / 3D / Video" />
      <SkillLine :level="94" skill="Legend of Zelda" />
    </div>
  </section>
</template>

<style lang="scss" scoped>
.skill-list {
  display: grid;
  gap: 1rem;
}
</style>
