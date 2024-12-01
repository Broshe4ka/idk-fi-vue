<script setup lang="ts">
import Control from './Control.vue';
</script>

<template>
  <div class="scene">
    <Control style="top: 40%; left: 70%" />
    <img
      src="https://i.pinimg.com/originals/86/8b/e7/868be70af8ebf3c9a8552c3409aa3919.png"
      alt="Beauty scene"
      class="scene__image"
    />
  </div>
</template>

<style scoped lang="scss">
.scene {
  position: absolute;
  width: 100%;
  height: 100%;
  border-radius: inherit;

  &__image {
    position: absolute;

    width: 100%;
    height: 100%;
    object-fit: cover;
    z-index: -1;
    border-radius: inherit;
  }
}
</style>
