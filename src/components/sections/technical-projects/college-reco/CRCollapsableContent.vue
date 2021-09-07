<template>
  <div class="about-container">
    <iframe src="https://collegereco.com/" width="750" height="460" />
  </div>
</template>
<script>
export default {
  name: "AboutCollapsableContent",
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
  padding: 15px;
  margin: 10px;
  
  background: white;
  box-shadow: 0 2px 2px 0 rgba(0, 0, 0, 0.14), 0 1px 5px 0 rgba(0, 0, 0, 0.12),
    0 3px 1px -2px rgba(0, 0, 0, 0.2);
}
</style>
