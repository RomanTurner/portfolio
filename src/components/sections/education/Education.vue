<template>
  <section class="container">
    <article class="intro-container">
      <p>
        <strong>Flatiron School</strong> - Seattle, WA - Full Stack Web
        Development Program
      </p>
      <p>02/02/2021 - 06/20/2021</p>
    </article>
    <article class="intro-container">
      <p>
        <strong>Utah State University</strong> - Logan, UT- Computer Science
      </p>
      <p>01/01/2011 - 04/01/2013</p>
    </article>
    <Collapsable buttonText="Show Certification">
      <EducationCollapsableContent
    /></Collapsable>
  </section>
</template>

<script>
import Collapsable from "../../basic-components/Collapsable.vue";
import EducationCollapsableContent from "./EducationCollapsableContent.vue";
export default {
  components: {
    Collapsable,
    EducationCollapsableContent,
  },
};
</script>

<style scoped>
.intro-container {
  display: flex;
  justify-content: space-between;
}
.container {
  width: 100%;
  text-align: left;
}
</style>
