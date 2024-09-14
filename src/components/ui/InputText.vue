<script lang="ts">
  export default {
    props: {
      text: {
        type: String,
        required: true
      }
    },
    data() {
      return {
        value: ""
      }
    },
    methods: {
      onClick(event){
        this.value = event.target.value
        this.text = this.value
      }
    }
  }
</script>

<template>
  <input
      v-bind:value="this.value"
      @input="this.onClick"
  />
</template>

<style scoped>

</style>