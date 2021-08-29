<template>
  <div class="button">
    {{ textContent }}
  </div>
</template>

<script>
export default {
  name: "button",
  props: {
    textContent: String,
  },
};
</script>
<style scoped>
.button {
  border: none;
  padding: 8px 64px;
  text-align: center;
  text-decoration: none;
  display: inline-block;
  font-size: 16px;
  margin: 2px 2px;
  transition-duration: 0.4s;
  cursor: pointer;
  background-color: white;
  color: black;
  border: 2px solid #77c9e7;
}
.button:hover {
  background-color: #77c9e7;
  color: white;
}
</style>
