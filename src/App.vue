<template>
  <div id="nav">
    <router-link to="/">Home</router-link>
    <router-link to="/about">About</router-link>
  </div>

  <div class="container">
    <router-view />
    <button class="btn btn--top-margin btn--center" @click="toggleModal">Modal</button>
    <div v-if="showModal">
      <Modal @close="toggleModal"></Modal>
    </div>
  </div>
</template>

<script>
import Modal from './components/Modal.vue'
export default {
  name: 'App',
  components: { Modal },
  data() {
    return {
      showModal: false,
    }
  },
  methods: {
    toggleModal() {
      this.showModal = !this.showModal
    },
  },
}
</script>



