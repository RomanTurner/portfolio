<template>
  <div class="home">
    <NavMenu @display-selected="currentTabComponent" />
    <main class="main">
      <section class="main-container">
        <Header />
        <transition name="fade" mode="out-in">
          <component :is="currentView"></component>
        </transition>
      </section>
    </main>
  </div>
</template>

<script>
// @ is an alias to /src
import NavMenu from "@/components/navigation/NavMenu.vue";
import Header from "@/components/sections/Header.vue";
import FullResume from "@/components/sections/FullResume.vue";
import TechnicalSkills from "@/components/sections/Skills.vue";
import TechnicalProjects from "@/components/sections/technical-projects/Projects.vue";
import AboutSection from "@/components/sections/about/About.vue";
import WorkExperience from "@/components/sections/work-experience/WorkExperience.vue";
import Education from "@/components/sections/education/Education.vue";

export default {
  components: {
    NavMenu,
    Header,
    FullResume,
    TechnicalSkills,
    TechnicalProjects,
    AboutSection,
    WorkExperience,
    Education,
  },
  data() {
    return {
      currentView: "FullResume",
    };
  },
  methods: {
    currentTabComponent({ id }) {
      console.log(this.currentView, id);
      this.currentView = id;
    },
  },
};
</script>

<style scoped>
.home {
  display: flex;
  justify-content: space-between;
  height: 95vh;
  overflow: hidden;
}
.main {
  width: 100%;
  display: flex;
  flex-direction: column;
  padding-left: 20px;
}
.main-container {
  background-color: white;
  display: flex;
  flex-direction: column;
  align-items: center;
  overflow: scroll;
}
.fade-enter-active,
.fade-leave-active {
  transition: opacity 0.5s;
}
.fade-enter, .fade-leave-to /* .fade-leave-active below version 2.1.8 */ {
  opacity: 0;
}
</style>
