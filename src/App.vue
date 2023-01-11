<template>
  <MenuComponent></MenuComponent>
  <p>esto es una prueba</p>
  <p>hola soy yo</p>
  <LogoComponent />
</template>

<script>
import MenuComponent from "@/components/MenuComponent.vue";
import LogoComponent from "@/components/LogoComponent.vue";
export default {
  name: "App",
  components: {
    MenuComponent,
    LogoComponent,
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
</style>
