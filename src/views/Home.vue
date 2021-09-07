<template>
  <WebView id="lg" />
  <MobileView id="sm" />
</template>

<script>
import MobileView from "./MobileView.vue";
import WebView from "./WebView.vue";

export default {
  name: "Home",
  components: {
    WebView,
    MobileView,
  },
};
</script>

<style scoped>
@media screen and (max-width: 800px) {
  #lg {
    display: none;
  }
  #sm {
    background-color: red;
  }
}
@media screen and (min-width: 800px) {
  #sm {
    display: none;
  }
}
</style>
