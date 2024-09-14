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

    background: transparent;
    color: #fff;
    border: none;

    box-shadow:0 0 0 1.5pt #535353 inset;

    font-size: 15pt;
  }

  button:hover {
    transition: 0.3s ease-in-out all;

    background: #535353;
  }

  button:active {
    transition: 0.1s ease-in-out all;
    transform: scale(0.95);

    background: #292929;
    box-shadow:0 0 0 1.5pt #292929 inset;
  }
</style>