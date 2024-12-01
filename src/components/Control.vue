<script setup lang="ts"></script>

<template>
  <div class="control">
    <input type="checkbox" class="control__dot" />
    <p class="control__title">Keyboard typing</p>
    <div class="control__volume">
      <input
        type="range"
        step="1"
        min="0"
        max="100"
        class="volume__range"
      />
      <span class="volume__text">100%</span>
    </div>
  </div>
</template>

<style lang="scss">
.control {
  position: absolute;
  display: flex;
  gap: 0.5rem;
  flex-direction: column;
  align-items: center;
  &__dot {
    position: relative;

    width: 2rem;
    height: 2rem;

    display: flex;
    align-items: center;
    justify-content: center;

    cursor: pointer;
    -webkit-appearance: none;
    appearance: none;

    filter: var(--main-shadow);
    &::before {
      content: '';
      position: absolute;
      width: 100%;
      height: 100%;
      border-radius: 100%;
      border: 2px solid var(--text-color);
    }
    &::after {
      content: '';
      position: absolute;
      width: 1.25rem;
      height: 1.25rem;
      background: var(--text-color);
      border-radius: 100%;
      opacity: 0;

      transition: var(--ease-transition);
    }
    &:checked::after {
      opacity: 1;
    }
  }
  &__title {
    filter: var(--main-shadow);
  }
  &__volume {
    display: flex;
    align-items: center;
    gap: 0.5rem;

    font-weight: 500;

    border-radius: 2rem;
    border: 1px solid rgba(255, 255, 255, 0.75);

    backdrop-filter: blur(8px);

    padding: 0.5rem 0.75rem;

    background: rgba(17, 17, 17, 0.2);
  }
}

// TODO: Style range

// .volume {
//   &__range {
//     background: transparent;
//     &::-moz-range-track {
//       border-radius: 0.5rem;
//       height: 8px;
//     }
//     &::-ms-track {
//       background: transparent;
//     }
//     &::-ms-fill-lower {
//       background: var(--text-color);
//       border-radius: inherit;
//     }
//     &::-ms-fill-upper {
//       background: #000;
//       border-radius: inherit;
//     }
//   }
//   &__text {
//   }
// }
</style>
