<template>
  <div class="about-container">
    <h3 class="title">Interests and Hobbies</h3>
    <div class="about-card" v-for="info in cardInfo" :key="info.id">
      <div
        class="card-image"
        :style="{ 'background-image': 'url(' + info.image + ')' }"
      ></div>
    </div>
  </div>
</template>
<script>
import puppyImage from "./assets/puppy.png";
import cooking1Image from "./assets/markit-meals2.png";

export default {
  name: "AboutCollapsableContent",
  data() {
    return {
      cardInfo: [
        {
          id: 1,
          textContent: "Puppy",
          image: puppyImage,
        },
        {
          id: 3,
          textContent: "Cooking1",
          image: cooking1Image,
        },
      ],
    };
  },
};
</script>

<style scoped>
.about-container {
  display: flex;
  flex-direction: column;
  justify-content: center;
  align-items: center;
  flex-wrap: wrap;
}
.about-card {
  width: 700px;
  height: 600px;
  padding: 10px;
  margin: 10px;
  background: white;
  box-shadow: 0 2px 2px 0 rgba(0, 0, 0, 0.14), 0 1px 5px 0 rgba(0, 0, 0, 0.12),
    0 3px 1px -2px rgba(0, 0, 0, 0.2);
}
.card-image {
  width: 100%;
  height: 100%;
  background-size: contain;
  background-repeat: no-repeat;
  background-position: center center;
}
h4 {
  margin: 5px;
}
</style>
