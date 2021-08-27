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
import TechnicalSkills from "@/components/TechnicalSkills.vue";
import TechnicalProjects from "@/components/TechnicalProjects.vue";
import AboutSection from "@/components/AboutSection.vue";
import WorkExperience from "@/components/WorkExperience.vue";
import Education from "@/components/Education.vue";

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
