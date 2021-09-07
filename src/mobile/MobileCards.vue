<template>
  <section class="container" v-for="card in cards" :key="card.id">
    <Collapsable :buttonText="card.title"
      ><p>{{ card.content }}</p></Collapsable
    >
  </section>
</template>
<script>
import Collapsable from "../components/basic-components/Collapsable.vue";

export default {
  name: "MobileCards",
  components: { Collapsable },
  data() {
    return {
      cards: [
        {
          id: 0,
          title: "About",
          content:
            "I am a JavaScript and Sushi enthusiast with a soft spot for Ruby and Musubi. I derive purpose from creation and I have a passion for making tools that can make your life easier. I am a community builder with ten years of experience working with small teams in production. I believe everyone has a unique skill or vision and I love seeing it piece together.",
        },
        {
          id: 1,
          title: "adf",
          content: "asdfaf",
        },
      ],
    };
  },
};
</script>
<style scoped>
.container {
  height: auto;
  overflow: hidden;
  width: 100%;
  padding: 10px;
  box-shadow: 0 2px 2px 0 rgba(0, 0, 0, 0.14), 0 1px 5px 0 rgba(0, 0, 0, 0.12),
    0 3px 1px -2px rgba(0, 0, 0, 0.2);
  margin-top: 10px;
}
</style>
