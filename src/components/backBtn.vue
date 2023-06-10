<script >
export default {
  name: 'backBtn',
  methods: {
    goBack() {
      window.history.length > 1 ? this.$router.go(-1) : this.$router.push('/')
    }
  }
}
</script>
<template>
  <div class="container-fluid p-sm-0">
    <svg id="btn-back" @click="goBack" viewBox="0 0 16 16" fill="#FFCA0D" xmlns="http://www.w3.org/2000/svg"
      class="bi bi-arrow-left-circle-fill">
      <path
        d="M8 0a8 8 0 1 0 0 16A8 8 0 0 0 8 0zm3.5 7.5a.5.5 0 0 1 0 1H5.707l2.147 2.146a.5.5 0 0 1-.708.708l-3-3a.5.5 0 0 1 0-.708l3-3a.5.5 0 1 1 .708.708L5.707 7.5H11.5z" />
    </svg>
  </div>
</template>
