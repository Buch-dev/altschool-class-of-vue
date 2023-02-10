<template>
  <h1>Color Picker Game</h1>

  <div>{{ message }}</div>

  <button v-for="color in colors" :key="color" @click="matchColor(color)">
    {{ color }}
  </button>
  <ColorPicker />

</template>

<script>
import { ref, reactive } from "@vue/reactivity";
import ColorPicker from '../composables/color-picker'

export default {
  name: "ColorPickerGame",
  components: {
    ColorPicker
  }
};
</script>

<style></style>
