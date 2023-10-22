<template>
  <div id="main-content">
    <Sidebar />
    <div id="dynamic-content">
      <slot />
    </div>
  </div>
</template>

<style>
#main-content {
  display: flex;
  height: 100vh;
  width: 100vw;
}

#dynamic-content {
  width: 75%;
  height: 100%;
  background: #f6f6f6;
  color: #333;
}

body {
  margin: 0;
  font-family: "Roboto", sans-serif;
}
</style>
