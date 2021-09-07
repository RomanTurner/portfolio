<template>
  <div class="nav-card">
    <span class="clicked">
      <h4>{{ event.title }}</h4>
    </span>
  </div>
</template>

<script>
export default {
  name: "NavMenuItem",
  props: {
    event: Object,
  },
};
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped>
.nav-card {
  padding: 15px;
  width: 250px;
  height: 60px;
  cursor: pointer;
  box-shadow: 0 3px 12px 0 rgba(0, 0, 0, 0.2);
}
.nav-card:hover {
  transform: scale(1.01);
  box-shadow: 0 3px 12px 0 rgba(0, 0, 0, 0.2);
}
</style>
