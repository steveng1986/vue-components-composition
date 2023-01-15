<template>
  <div>
    <button @click="toggle">Boton Modal</button>
    <teleport to="body">
      <div v-show="showModal" class="modal-container">
        <h1>title</h1>
        <p>Lorem, ipsum dolor.</p>
        <button @click="toggle">Boton Modal</button>
      </div>
    </teleport>
  </div>
</template>

<script>
export default {
  data() {
    return {
      showModal: false,
    };
  },
  methods: {
    toggle() {
      if (this.showModal === true) {
        this.showModal = false;
      } else {
        this.showModal = true;
      }
    },
  },
};
</script>
