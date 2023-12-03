<template>
  <div class="main">
    <div class="content">
      <p class="title">{{ title }}</p>
      <div class="description">{{ description }}</div>
      <div id="technologyContainer">
        <div id="technologyTitle">Technologies</div>
        <div id="technologyList">
          <span v-for="technology in technologies" :key="technology">
            {{ technology }},
          </span>
        </div>
      </div>
      <a :href="link" target="__blank">
        <Button text="Learn More" theme="dark" mt="20" />
      </a>
    </div>
    <div class="image">
      <img :src="imageSrc" :alt="title" />
    </div>
  </div>
</template>

<script>
export default {
  props: {
    title: String,
    description: String,
    technologies: Array,
    link: String,
    imageSrc: String,
    buttonText: String,
  },
};
</script>

<style scoped>
img {
  max-width: 100%;
  max-height: 568px;
}

.main {
  display: flex;
}

.image {
  width: 100%;
  padding-left: 0;
}

.content {
  width: 50%;
}

.title {
  margin: 0;
  font-weight: 500;
  font-size: 22px;
  color: #40748a;
}

.description {
  margin-top: 20px;
}
</style>
