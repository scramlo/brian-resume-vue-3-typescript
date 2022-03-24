<script setup lang="ts">
import SectionTitle from "@/components/SectionTitle.vue";
import InfoGroup from "@/components/InfoGroup.vue";
import { CIcon } from "@coreui/icons-vue";
import { cilPhone, cilEnvelopeLetter, cilHouse } from "@coreui/icons";
import SvgLine from "@/components/SvgLine.vue";
</script>
<template>
  <section class="contact">
    <SectionTitle title="Contact" />
    <InfoGroup>
      <template #icon>
        <CIcon :icon="cilPhone" />
      </template>
      <template #title>
        <strong>Phone:</strong>
      </template>
      <template #info> +1 269 317 1160 </template>
    </InfoGroup>
    <SvgLine
      class="contact__separator"
      :width="100"
      color="var(--brian-dark)"
    />
    <InfoGroup>
      <template #icon>
        <CIcon :icon="cilEnvelopeLetter" />
      </template>
      <template #title>
        <strong>Email:</strong>
      </template>
      <template #info>brian@nerdspecs.com</template>
    </InfoGroup>
    <SvgLine
      class="contact__separator"
      :width="100"
      color="var(--brian-dark)"
    />
    <InfoGroup>
      <template #icon>
        <CIcon :icon="cilHouse" />
      </template>
      <template #title>
        <strong>Address:</strong>
      </template>
      <template #info>
        <address>
          540 Minges Road E<br />
          Battle Creek, MI<br />
          49015
        </address>
      </template>
    </InfoGroup>
  </section>
</template>

<style scoped lang="scss">
.contact {
  &__separator {
    margin: 1rem 0;
  }
}
</style>
