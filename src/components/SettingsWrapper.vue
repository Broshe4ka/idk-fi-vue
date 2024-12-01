<script setup lang="ts">
import AdittionalMenu from './ui/menu/AdittionalMenu.vue';
// import ScenesMenu from './ui/menu/ScenesMenu.vue';
// import SettingsMenu from './ui/menu/SettingsMenu.vue';
</script>

<template>
  <div class="menu-wrapper">
    <AdittionalMenu />
    <!-- <ScenesMenu /> -->
    <!-- <SettingsMenu /> -->
  </div>
</template>

<style scoped lang="scss">
.menu-wrapper {
  max-width: 600px;
  width: 100%;
  display: flex;
  align-items: center;
  justify-content: flex-start;

  padding: 1rem;

  border-radius: 0.75rem;

  background: #111111bf;
  backdrop-filter: blur(8px);
}
</style>
