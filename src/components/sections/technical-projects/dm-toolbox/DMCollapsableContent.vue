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
import charEdit from "./assets/char-edit.gif";
import monsters from "./assets/monsters.gif";
import noteEdit from "./assets/note-edit.gif";
import npc from "./assets/npc.gif";
import campaingPng from "./assets/campaign.png";
import charNotes from "./assets/character-notes.png";
import itemCustomisation from "./assets/item-custom.png";

export default {
  name: "AboutCollapsableContent",
  data() {
    return {
      cardInfo: [
        {
          id: 1,
          textContent: "Campain Dashboard",
          image: campaingPng,
        },
        {
          id: 2,
          textContent: "Character Edit",
          image: charEdit,
        },
        {
          id: 3,
          textContent: "Character Notes",
          image: charNotes,
        },
        {
          id: 4,
          textContent: "Item customization",
          image: itemCustomisation,
        },
        {
          id: 5,
          textContent: "Quick Monser Lookup",
          image: monsters,
        },
        {
          id: 6,
          textContent: "Campain Note Editing",
          image: noteEdit,
        },
        {
          id: 7,
          textContent: "NPC Randomizer",
          image: npc,
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
  margin-left: 100px;
  width: 500px;
  height: 80%;
  background-size: cover;
  background-repeat: no-repeat;
  background-position: center center;
}
h4 {
  margin: 5px;
}
</style>
