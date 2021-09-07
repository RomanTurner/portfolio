<template>
  <nav class="nav">
    <div>Hello</div>
    <img :src="image" alt="laptop demo" />
  </nav>
</template>

<script>
import recipeShowLaptop from "@/mobile/assets/flavorites-laptop.gif";

export default {
  name: "MobileMenu",
  data() {
    return {
      image: recipeShowLaptop,
      events: [
        {
          id: "FullResume",
          title: "Full Resume",
        },
        {
          id: "AboutSection",
          title: "About Me",
        },
        {
          id: "TechnicalSkills",
          title: "Technical Skills",
        },
        {
          id: "TechnicalProjects",
          title: "Technical Projects",
        },
        {
          id: "WorkExperience",
          title: "Work Experience",
        },
        {
          id: "Education",
          title: "Education",
        },
      ],
    };
  },
};
</script>

<style scoped>
.nav {
  display: flex;
  flex-direction: column;
  align-items: left;
}
.nav:nth-child(even) {
  background-color: #ebebeb;
}
.nav:nth-child(odd) {
  background-color: #77c9e7;
}
.decorative {
  background-color: #77c9e7;
  padding-left: 20px;
  padding-bottom: 20px;
  overflow: auto;
}
</style>
