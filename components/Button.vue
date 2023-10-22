<template>
  <button class="custom-button">
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
  },
};
</script>

<style scoped>
.custom-button {
  background-color: transparent;
  color: #ffffff;
  border: 2px solid #ffffff;
  padding: 10px 20px;
  cursor: pointer;
  border-radius: 5px;
  font-size: 16px;
  transition:
    background-color 0.3s,
    color 0.3s;
}

.custom-button:hover {
  background-color: #ffffff;
  color: #000000;
}
</style>
