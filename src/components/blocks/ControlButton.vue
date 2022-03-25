<script lang="ts" setup>
import { CIcon } from "@coreui/icons-vue";
import { cilSettings } from "@coreui/icons";
</script>
<template>
  <button class="control-button">
    <CIcon :icon="cilSettings" />
  </button>
</template>

<style scoped lang="scss">
.control-button {
  position: fixed;
  height: 50px;
  width: 50px;
  background-color: var(--brian-accent);
  top: 2rem;
  right: 2rem;
  z-index: 1;
  border-radius: 100%;
  border: none;
  padding: 0.5rem;
  box-shadow: 0 3px 5px rgba(0, 0, 0, 0.5);
  cursor: pointer;

  @keyframes spin {
    0% {
      transform: rotate3d(0, 0, 0, 0);
    }

    100% {
      transform: rotate3d(1, 0, 0, -180deg);
    }
  }

  &:hover {
    animation: spin 1s;
  }

  &:active {
    transform: translate3d(3px, 3px, 3px);
  }
}
</style>
