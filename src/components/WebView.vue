<template>
  <div class="home">
    <NavMenu @display-selected="currentTabComponent" />
    <main class="main">
      <Header />
      <section class="main-container">
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
import Header from "@/components/Header.vue";
import FullResume from "@/components/FullResume.vue";
import TechnicalSkills from "@/components/TechnicalSkills.vue";
import TechnicalProjects from "@/components/TechnicalProjects.vue";
import AboutSection from "@/components/AboutSection.vue";
import WorkExperience from "@/components/WorkExperience.vue";
import Education from "@/components/Education.vue";

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
      console.log(this.currentView, id)
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
