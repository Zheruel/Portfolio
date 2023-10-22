<template>
  <div id="sidebar-container">
    <div id="overlay">
      <NuxtLink to="/">
        <Avatar width="160" height="160" url="/tin.png" />
      </NuxtLink>
      <p id="name">Tin Zeljar</p>
      <p id="title">Software Engineer</p>
      <button @click="incrementCounter">Click me!</button>
      <p>Counter: {{ counter }}</p>
    </div>
  </div>
</template>

<script setup>
const counter = ref(0);

function incrementCounter() {
  counter.value++;
}
</script>

<style>
p {
  color: #fff;
}

#sidebar-container {
  width: 25%;
  height: 100%;
  background: url("/background.jpg") no-repeat center center/cover;
  position: relative;
}

#overlay {
  padding: 45px 40px;
  box-sizing: border-box;
  position: absolute;
  top: 0;
  left: 0;
  width: 100%;
  height: 100%;
  background-color: rgba(0, 0, 0, 0.6);
}

#name {
  font-size: 24px;
  font-weight: bold;
  margin-top: 10px;
  text-align: center;
  text-transform: uppercase;
}

#title {
  font-size: 16px;
  margin-top: -20px;
  text-align: center;
  text-transform: uppercase;
}
</style>
