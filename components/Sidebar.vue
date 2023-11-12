<template>
  <div id="sidebar-container">
    <div id="overlay">
      <NuxtLink to="/">
        <Avatar width="160" height="160" url="/tin.png" />
        <p id="name">Tin Zeljar</p>
        <p id="title">Software Engineer</p>
      </NuxtLink>

      <div id="menu">
        <NuxtLink
          to="/portfolio"
          exact
          active-class="active-link"
          class="menu-link"
        >
          <p>Portfolio</p>
        </NuxtLink>
        <NuxtLink
          to="/offer"
          exact
          active-class="active-link"
          class="menu-link"
        >
          <p>My Offer</p>
        </NuxtLink>
        <NuxtLink
          to="/contact"
          exact
          active-class="active-link"
          class="menu-link"
        >
          <p>Contact me</p>
        </NuxtLink>
        <a
          href="https://drive.google.com/file/d/1rlqsZ7fER3EZJ4cWicx-g_y1o3CBoj7D/view?usp=sharing"
          target="__blank"
          class="menu-link"
        >
          <p>Get my cv</p>
        </a>
      </div>
    </div>
  </div>
</template>

<style>
a {
  text-decoration: none;
}

p {
  color: #fff;
}

#sidebar-container {
  width: 16%;
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

#menu {
  margin-top: 50px;
  text-align: center;
  text-transform: uppercase;
  font-size: 18px;
}

.menu-link {
  display: block;
  margin-bottom: 10px;
  border-radius: 5px;

  :hover {
    opacity: 0.5;
  }
}

.active-link {
  opacity: 0.5;
}
</style>
