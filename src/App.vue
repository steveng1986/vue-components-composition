<template>
  <div>{{ text }}</div>
  <div>{{ algo }}</div>
</template>

<script>
import base from "@/mixines/base";
export default {
  name: "App",
  mixins: [base],
  components: {},
  data() {
    return {
      text: "Hola soy una variable",
    };
  },
  beforeCreate() {
    console.log("soy before create", this.$data, this.$el);
  },
  created() {
    console.log("soy created", this.$data, this.$el);
  },
  mounted() {
    console.log("soy mounted", this.$data, this.$el);
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
