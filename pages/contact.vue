<template>
  <div id="contact-section">
    <h1>Contact me</h1>
    <p>I'm open to hear about interesting proposals.</p>

    <div class="flex-container" style="margin: 30px 0 20px 0">
      <p class="contact-section-label">E-mail:</p>
      <a href="mailto:tinzeljar@gmail.com">
        <Icon name="ic:baseline-email" class="contact-icon" />
        tinzeljar@gmail.com
      </a>
    </div>

    <div class="flex-container">
      <p class="contact-section-label">LinkedIn:</p>
      <a href="https://www.linkedin.com/in/tin-zeljar/" target="_blank">
        <Icon name="akar-icons:linkedin-fill" class="contact-icon" />
        Tin Zeljar
      </a>
    </div>

    <div class="flex-container">
      <p class="contact-section-label">GitHub:</p>
      <a href="https://github.com/Zheruel" target="_blank">
        <Icon name="akar-icons:github-fill" class="contact-icon" />
        Tin Zeljar
      </a>
    </div>
  </div>
</template>

<style scoped>
p {
  color: #555;
}

h1 {
  margin: 0;
  text-transform: uppercase;
  font-weight: 400;
}

a {
  text-decoration: none;
  color: #40748a;
}

a:hover {
  opacity: 0.8;
}

#contact-section {
  padding: 50px;
  max-width: 850px;
  background-color: white;
  color: #555;

  @media screen and (max-width: 1024px) {
    padding: 30px 20px;
  }
}

.flex-container {
  display: flex;
  align-items: center;
}

.contact-icon {
  color: #40748a;
  margin-right: 5px;
  font-size: 20px;
}

.contact-section-label {
  width: 50px;
  margin: 0 100px 5px 0;

  @media screen and (max-width: 1024px) {
    width: 50px;
    margin: 0 60px 5px 0;
  }
}
</style>
