<template>
  <div class="about-container">
    <h3 class="title">Flavorites - Meal Planning Features</h3>
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
import addRecipe from "./assets/add-recipe.gif";
import dashboard from "./assets/meal-plan-dash.gif";
import index from "./assets/mealplan-index.gif";
import crudActions from "./assets/mp-crud.gif";
import recipeShow from "./assets/recipe-show.gif";
import searchPagination from "./assets/search-pagination.gif";

export default {
  name: "AboutCollapsableContent",
  data() {
    return {
      cardInfo: [
        {
          id: 1,
          textContent: "Meal Plan Dashboard",
          image: dashboard,
        },
        {
          id: 2,
          textContent: "User Meal Plans",
          image: index,
        },
        {
          id: 3,
          textContent: "Recipe Description Page",
          image: recipeShow,
        },
        {
          id: 4,
          textContent: "Adding a Recipe",
          image: addRecipe,
        },
        {
          id: 5,
          textContent: "Meal Plan CRUD",
          image: crudActions,
        },
        {
          id: 6,
          textContent: "Search Indexing and Pagination",
          image: searchPagination,
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
  border-radius: 5%;
  background: white;
  box-shadow: 0 2px 2px 0 rgba(0, 0, 0, 0.14), 0 1px 5px 0 rgba(0, 0, 0, 0.12),
    0 3px 1px -2px rgba(0, 0, 0, 0.2);
}
.card-image {
  width: 100%;
  height: 80%;
  background-size: contain;
  background-repeat: no-repeat;
  background-position: center center;
}
h4 {
  margin: 5px;
}
</style>
