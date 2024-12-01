<script setup lang="ts"></script>

<template>
  <div class="additional">
    <div class="additional__button">
      <span>Pomodoro</span>
      <!-- <img src="" alt="" /> -->
    </div>
    <div class="additional__button">
      <span>Tasks</span>
      <!-- <img src="" alt="" /> -->
    </div>
    <div class="additional__button">
      <span>Planer</span>
      <!-- <img src="" alt="" /> -->
    </div>
    <div class="additional__button">
      <span>idk</span>
      <!-- <img src="" alt="" /> -->
    </div>
  </div>
</template>

<style scoped lang="scss">
.additional {
  width: 100%;
  display: flex;
  flex-wrap: wrap;
  gap: 1rem;
  &__button {
    aspect-ratio: 16 / 9;
    width: calc(50% - 0.5rem);

    display: flex;
    align-items: center;
    justify-content: center;

    text-align: center;
    font-family: Comfortaa;
    font-size: 2.5rem;
    font-weight: 500;
    letter-spacing: -2px;

    border-radius: 0.5rem;
    background: #191919;
  }
}
</style>
