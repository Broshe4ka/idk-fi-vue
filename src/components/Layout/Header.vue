<script setup lang="ts"></script>

<template>
  <div class="header">
    <span class="header__logo">idk-fi</span>
  </div>
</template>

<style lang="scss">
.header {
  position: relative;

  font-family: 'Comfortaa', sans-serif;
  font-size: 3rem;
  font-weight: 700;
  letter-spacing: -2.4px;

  display: flex;
  align-self: flex-start;
  padding: 5px 1.5rem;

  border-radius: 0 0 1rem 0;

  background: var(--main-bg);

  z-index: var(--z-index-higher);

  &::after,
  &::before {
    content: '';
    position: absolute;
    width: 1rem;
    height: 1rem;
    background: url(/icons/rec.svg);
    transform: rotate(90deg);
  }
  &::after {
    top: 0;
    right: -1rem;
  }
  &::before {
    bottom: -1rem;
    left: 0;
  }
}
</style>
