<template>
  <nav class="nav">
    <Avatar />
    <div class="decorative">
      <NavMenuItem
        @click="$emit('display-selected', event)"
        class="nav"
        v-for="event in events"
        :key="event.id"
        :event="event"
      />
    </div>
  </nav>
</template>

<script>
// @ is an alias to /src
import NavMenuItem from "@/components/navigation/NavMenuItem.vue";
import Avatar from "@/components/navigation/Avatar.vue";

export default {
  name: "NaveMenu",
  emits: ["display-selected"],
  components: {
    NavMenuItem,
    Avatar,
  },
  data() {
    return {
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
