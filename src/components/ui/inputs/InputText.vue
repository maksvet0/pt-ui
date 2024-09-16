<script lang="ts">
  export default {
    props: {
      placeholder: {
        type: String,
        required: false,
      }
    },
    data() {
      return {
        value: ""
      }
    },
    emits: ['on-change'],
    methods: {
      onChangeEvent(event){
        this.value = event.target.value
        this.$emit("on-change", this.value)
      }
    }
  }
</script>

<template>
  <input
      :placeholder="this.placeholder"
      type="text"
      :value="this.value"
      @input="this.onChangeEvent"
  />
</template>

<style scoped>
  input[type=text] {
    background: #303030;
    border: solid 2pt #828282;
    border-radius: 5pt;
    padding: 5pt 15pt;

    color: #fff;
    font-size: 15pt;
    font-weight: normal;
    outline: none;
  }

</style>