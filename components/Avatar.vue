<template>
  <header class="avatar">
    <img :src="url" :width="width" :height="height" alt="Header Image" />
  </header>
</template>

<script>
export default {
  props: {
    url: {
      type: String,
      required: true,
    },
    width: {
      type: [String, Number],
      default: 50,
    },
    height: {
      type: [String, Number],
      default: 50,
    },
  },
};
</script>

<style scoped>
.avatar {
  padding: 10px;
  text-align: center;
}

.avatar img {
  border-radius: 50%;
}
</style>
