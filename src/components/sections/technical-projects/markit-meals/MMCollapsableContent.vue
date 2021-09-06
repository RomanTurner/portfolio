<template>
  <div class="about-container">
    <h3 class="title">Markit Meal-kit Service</h3>
    <div class="about-card" v-for="info in cardInfo" :key="info.id">
      <h4>{{ info.textContent }}</h4>
      <div
        class="card-image"
        :style="{ 'background-image': 'url(' + info.image + ')' }"
      ></div>
    </div>
  </div>
</template>
<script>
import mm1 from "./assets/markit-meals.png";
import mm2 from "./assets/markit-meals2.png";

export default {
  name: "AboutCollapsableContent",
  data() {
    return {
      cardInfo: [
        {
          id: 5,
          textContent: "Pike Place Market",
          image: mm1,
        },
        {
          id: 1,
          textContent: "Locally Sourced Meals",
          image: mm2,
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
  height: 400px;
  padding: 10px;
  margin: 10px;
  background: white;
  box-shadow: 0 2px 2px 0 rgba(0, 0, 0, 0.14), 0 1px 5px 0 rgba(0, 0, 0, 0.12),
    0 3px 1px -2px rgba(0, 0, 0, 0.2);
}
.card-image {
  width: 100%;
  height: 90%;
  background-size: cover;
  background-repeat: no-repeat;
  background-position: center center;
}
h4 {
  margin: 5px;
}
</style>
