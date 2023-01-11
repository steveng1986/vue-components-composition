<template>
  <button @click="show = !show">Menu</button>
  <transition name="fade">
    <MenuMenu v-show="show" />
  </transition>
</template>

<script>
import MenuMenu from "@/components/MenuMenu.vue";
export default {
  name: "App",
  components: { MenuMenu },

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
