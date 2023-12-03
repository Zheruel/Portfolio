<template>
  <button
    class="custom-button"
    :class="{
      'light-theme': theme === 'light',
      'dark-theme': theme === 'dark',
    }"
    :style="{ marginTop: mt + 'px' }"
  >
    {{ text }}
  </button>
</template>

<script>
export default {
  props: {
    text: {
      type: String,
      required: true,
    },
    theme: {
      type: String,
      default: "light",
    },
    mt: {
      type: [Number, String],
      default: 0,
    },
  },
};
</script>

<style scoped>
.custom-button {
  padding: 10px 20px;
  cursor: pointer;
  border-radius: 5px;
  font-size: 16px;
  transition:
    background-color 0.3s,
    color 0.3s;
}

.light-theme {
  background-color: transparent;
  color: #ffffff;
  border: 2px solid #ffffff;
}

.light-theme:hover {
  background-color: #ffffff;
  color: #40748a;
}

.dark-theme {
  background-color: #40748a;
  color: #ffffff;
  border: 2px solid #40748a;
}

.dark-theme:hover {
  background-color: #ffffff;
  color: #40748a;
}
</style>
