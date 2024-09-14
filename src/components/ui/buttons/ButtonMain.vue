<script lang="ts">
  export default {
    props: {
      title: {
        type: String,
        required: true
      },
      onClick: {
        type: Function,
        required: false
      }
    }
  }
</script>

<template>
  <button @click="this.onClick">
    {{ this.title }}
  </button>
</template>

<style scoped>
  button {
    transition: 0.3s ease-in-out all;
    cursor: pointer;
    padding: 5pt 25pt;
    border-radius: 5pt;

    background: #2e2e2e;
    color: #fff;
    border: none;

    font-size: 15pt;
  }

  button:hover {
    transition: 0.3s ease-in-out all;
    box-shadow: 0 0 30pt 5px rgba(124, 181, 63, 0.6);

    background: #7cb53f;
  }

  button:active {
    transition: 0.1s ease-in-out all;

    transform: scale(0.95);
    background: #415e25;
  }
</style>