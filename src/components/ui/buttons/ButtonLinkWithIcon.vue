<template>
  <button
      @click="onClick"
      :class="styleClass"
  >
    <!-- Добавляем класс для иконки и стилизуем его -->
    <slot name="icon" class="icon"></slot>
    <span/>
    {{ title }}
  </button>
</template>

<script lang="ts">
export default {
  props: {
    title: {
      type: String,
      required: true,
    },
    onClick: {
      type: Function,
      required: false,
    },
    styleClass: {
      type: String,
      required: false,
    },
  },
};
</script>

<style scoped>

span {
  width: 15pt;
}

button {
  padding: 5pt;
  display: flex;
  align-items: center;
  transition: 0.3s ease-in-out all;
  cursor: pointer;
  border-radius: 5pt;
  background: transparent;
  color: rgba(255, 255, 255, 0.70);
  border: none;
  font-size: 15pt;
  font-weight: 500;
}


button:hover {
  transition: 0.3s all;
  text-shadow: 0 0 12pt rgba(44, 202, 0, 0.81);
  transform: scale(1.1);
  color: rgb(255, 255, 255);
}

button:active {
  transition: 0.2s ease-in-out all;
  transform: scale(0.95);
}
</style>

