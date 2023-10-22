<template>
  <div id="background">
    <div id="hero">
      <h1 id="intro">Hi, I'm Tin.</h1>
      <p id="description">
        A skilled software engineer with over
        <b>{{ dateDifference }} years of experience</b> specialized in both
        <b>front end</b> and <b>back end</b>.
      </p>
      <div id="button-container">
        <NuxtLink to="/portfolio">
          <Button text="Portfolio" />
        </NuxtLink>
        <NuxtLink to="/offer">
          <Button text="My offer" />
        </NuxtLink>
        <NuxtLink to="/offer">
          <Button text="Grab CV" />
        </NuxtLink>
      </div>
    </div>
  </div>
</template>

<script setup>
const dateDifference = new Date().getFullYear() - 2018;
</script>

<style scoped>
#background {
  padding: 160px 0 0 60px;
  box-sizing: border-box;
  width: 100%;
  height: 100%;
  background-image: url("/background.jpg");
  background-repeat: no-repeat;
  background-size: cover;
  background-position: center;
}

#hero {
  text-shadow: 0 4px 4px rgba(0, 0, 0, 0.25);
  color: white;
  opacity: 0;
  animation: fadeIn 1s ease-in-out forwards;
}

#intro {
  margin: 0;
  font-size: 60px;
}

#description {
  max-width: 650px;
  font-size: 30px;
}

#button-container {
  display: flex;
  gap: 20px;
}

@keyframes fadeIn {
  from {
    opacity: 0;
  }
  to {
    opacity: 1;
  }
}
</style>
