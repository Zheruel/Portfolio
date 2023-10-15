<template>
  <div id="sidebar-container">
    <Avatar
      width="100"
      height="100"
      url="https://www.codeproject.com/KB/testing/1002904/Test-URL-Redirects-HttpWebRequest.jpg"
    />
    <button @click="incrementCounter">Click me!</button>
    <p>Counter: {{ counter }}</p>
  </div>
</template>

<script setup>
const counter = ref(0);

function incrementCounter() {
  counter.value++;
}
</script>

<style>
#sidebar-container {
  position: fixed;
  top: 0;
  left: 0;
  width: 25%;
  height: 100%;
  background-color: #333;
  color: #fff;
}
</style>
