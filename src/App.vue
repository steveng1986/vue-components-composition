<template>
  <ModalComponent></ModalComponent>
</template>

<script>
import ModalComponent from "@/components/ModalComponent.vue";
export default {
  name: "App",
  components: {
    ModalComponent,
  },
  data() {
    return {
      show: false,
    };
  },
};
</script>

<style lang="scss">
#app {
  font-family: Avenir, Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  text-align: center;
  color: #2c3e50;
  margin-top: 60px;
}
.fade-enter-from,
.fade-leave-to {
  opacity: 0;
}

.fade-enter-active,
.fade-leave-active {
  transition: opacity 0.5s ease;
}
</style>
