<template>
  <section>
    <AboutSection />
    <hr />
    <TechnicalSkills />
    <hr />
    <TechnicalProjects />
    <hr />
    <WorkExperience />
    <hr />
    <Education />
    <hr />
  </section>
</template>

<script>
// @ is an alias to /src
import AboutSection from "@/components/sections/about/About.vue";
import Education from "@/components/sections/Education.vue";
import TechnicalSkills from "@/components/sections/Skills.vue";
import TechnicalProjects from "@/components/sections/technical-projects/Projects.vue";
import WorkExperience from "@/components/sections/WorkExperience.vue";

export default {
  name: "FullResume",
  components: {
    TechnicalSkills,
    TechnicalProjects,
    AboutSection,
    WorkExperience,
    Education,
  },
};
</script>

<style scoped>
hr {
  border: solid 1px #ebebeb;
  border-top: 2px solid #77c9e7;
  border-bottom: 1px solid black;
  width: 85%;
}
</style>
