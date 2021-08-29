<template>
  <div class="about-container">
    <h3 class="title">Interests and Hobbies</h3>
    <div class="about-card" v-for="info in cardInfo" :key="info.id">
      <h4>{{ info.textContent }}</h4>
      <img class="card-image" :src="info.image" />
    </div>
  </div>
</template>
<script>
import image1 from "../../../assets/logo.png"; 

export default {
  name: "AboutCollapsableContent",
  data() {
    return {
      cardInfo: [
        {
          id: 1,
          textContent: "Biking",
          image: image1,
        },
        {
          id: 2,
          textContent: "Cooking",
          image: image1,
        },
        {
          id: 3,
          textContent: "Reading",
          image: image1,
        },
        {
          id: 4,
          textContent: "Hello",
          image: image1,
        },
        {
          id: 4,
          textContent: "Hello",
          image: image1,
        },
        {
          id: 4,
          textContent: "Hello",
          image: image1,
        },
      ],
    };
  },
};
</script>

<style scoped>
.about-container {
  display: flex;
  flex-direction: row;
  justify-content: space-around;
  flex-wrap: wrap;
}
.about-card {
  width: 200px;
  height: 150px;
  padding: 10px;
  margin: 10px;
  background: white;
  border-radius: 5%;
  box-shadow: 0 2px 2px 0 rgba(0, 0, 0, 0.14), 0 1px 5px 0 rgba(0, 0, 0, 0.12),
    0 3px 1px -2px rgba(0, 0, 0, 0.2);
}
.card-image {
  height: 100px;
}
.title {
  width: 100%;
}
h4 {
  margin: 5px;
}
</style>
