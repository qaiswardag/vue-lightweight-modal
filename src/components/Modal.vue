<template>
  <div class="modal" @click.self="closeModal">
    <div class="modal-container">
      <h3>consectetur adipisicing</h3>
      <p>
        Lorem ipsum dolor, sit amet consectetur adipisicing elit. Rerum et
        officiis saepe.
      </p>
      <form action="">
        <label>soluta totam</label>
        <input type="text" placeholder="soluta totam">
        <label>soluta totam</label>
        <input type="text" placeholder="inventore">
        <button class="btn btn--top-margin">submit</button>
      </form>
    </div>
  </div>
</template>


<script>
export default {
  methods: {
    closeModal() {
      this.$emit('close')
    },
  },
}
</script>
