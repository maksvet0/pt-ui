<script setup lang="ts">
  import ButtonMain from "@/components/ui/buttons/ButtonMain.vue";
  import ButtonSecond from "@/components/ui/buttons/ButtonSecond.vue";
  import ButtonLink from "@/components/ui/buttons/ButtonLink.vue";
  import InputText from "@/components/ui/InputText.vue";
  // imports here
</script>

<script lang="ts">
  let value = ""
  function i(){
    alert(this.value)
  }
  // scripts here
</script>

<template>
  <div>
    <ButtonMain title="Hello! I'm Main Button"/>
    <br>
    <ButtonSecond title="Hello! I'm Second Button"/>
    <br>
    <ButtonLink title="Hello! I'm Link Button" :on-click="i"/>
    <InputText />
  </div>
  <!-- html here -->
</template>

<style>
  @import url('https://fonts.googleapis.com/css2?family=Jost:ital,wght@0,100..900;1,100..900&display=swap');

  button {
    margin: 5pt;
  }

  * {
    font-family: "Jost", serif;
  }

  body {
    background-color: #1A1A1A;
  }
</style>