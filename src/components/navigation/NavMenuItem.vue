<template>
  <div class="nav-card">
    <h4>{{ event.title }}</h4>
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
  cursor: pointer;
}
.nav-card:hover {
  transform: scale(1.01);
  box-shadow: 0 3px 12px 0 rgba(0, 0, 0, 0.2);
}
.clicked {
  position: absolute;
  border-radius: 50%;
  transform: scale(0);
  animation: ripple 600ms linear;
  background-color: rgba(255, 255, 255, 0.7);
}
@keyframes ripple {
  to {
    transform: scale(4);
    opacity: 0;
  }
}
</style>
