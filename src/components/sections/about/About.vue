<template>
  <article class="intro-container">
    <p>
      I am a JavaScript and Sushi enthusiast with a soft spot for Ruby and
      Musubi. I derive purpose from creation and I have a passion for making
      tools that can make your life easier. I am a community builder with ten
      years of experience working in and as a manager of small teams. I believe
      everyone has a unique skill or vision and I love seeing it piece together.
    </p>
    <Collapsable buttonText="More About Me">
      <AboutCollapsableContent />
    </Collapsable>
  </article>
</template>
<script>
import Collapsable from "../../basic-components/Collapsable.vue";
import AboutCollapsableContent from "./AboutCollapsableContent.vue";
export default {
  name: "About",
  components: {
    Collapsable,
    AboutCollapsableContent,
  },
};
</script>
<style scoped>
.intro-container {
  display: flex;
  flex-direction: column;
  align-items: flex-start;
  text-align: left;
  width: 100%;
}
p {
  margin: 5px;
}
</style>
