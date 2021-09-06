<template>
  <div class="collapsable">
    <CustomButton
      @click="onClick"
      :style="{ alignSelf: 'center' }"
      :textContent="open ? 'Close' : buttonText"
    />
    <transition name="fade">
      <div class="collapsable-content" v-if="open">
        <slot></slot>
      </div>
    </transition>
  </div>
</template>

<script>
import CustomButton from "./CustomButton.vue";
export default {
  name: "Collapsable",
  components: { CustomButton },
  props: ["buttonText"],
  data() {
    return {
      open: false,
    };
  },
  methods: {
    onClick() {
      this.open = !this.open;
    },
  },
};
</script>
<style scoped>
.fade-enter-active {
  transition: all 0.2s cubic-bezier(0.55, 0.085, 0.68, 0.53);
  transform-origin: 50% 50%;
}
.fade-leave-active {
  transform-origin: 50% 50%;
  transition: all 0.5s cubic-bezier(0.25, 0.46, 0.45, 0.94);
}

.fade-enter-from,
.fade-leave-to {
  transform-origin: 50% 50%;
  transform: scaleY(0) translateZ(0);
  opacity: 0;
}
.collapsable {
  top: -1px;
  display: flex;
  flex-direction: column;
  width: 100%;
  overflow: hidden;
}
.collapsable-content {
  margin-top: 10px;
  background-color: #ebebeb;
  width: 100%;
  height: 475px;
  text-align: center;
  overflow: scroll;
}
</style>
