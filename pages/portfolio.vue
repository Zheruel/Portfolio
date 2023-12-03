<template>
  <div id="portfolio-section">
    <h1>Portfolio</h1>
    <p>Looking for a full-stack engineer who can develop your idea?</p>
    <p>
      Let's tackle your unique challenges
      <NuxtLink class="highlight" to="/contact"> together</NuxtLink>
      .
    </p>
    <hr />
    <h2>Projects</h2>
    <ProjectItem
      title="Bachelor's Thesis Project"
      description="Web shop created using .NET Core as the back-end and JavaScript with JQuery as the front-end."
      :technologies="[
        'HTML/CSS',
        'JavaScript',
        'jQuery',
        'C#',
        'ASP.NET',
        'MsSQL',
      ]"
      link="https://github.com/Zheruel/Mr-Robot-Webshop"
      imageSrc="~/assets/webshop.jpg"
    />
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

h2 {
  text-transform: uppercase;
  font-weight: 400;
  font-size: 26px;
}

#portfolio-section {
  padding: 50px;
  max-width: 1400px;
  background-color: white;
  color: #555;

  @media screen and (max-width: 1024px) {
    padding: 30px 20px;
  }
}

.highlight {
  font-weight: bold;
  color: #40748a;
}
</style>
