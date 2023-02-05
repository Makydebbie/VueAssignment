<template>
  <div> <h1>Color Picker Game</h1>
  
    <div>{{ message }}</div>
  
    <button v-for="color in colors" :key="color" @click="matchColor(color)">
      {{ color }}
    </button></div> 
  </template>
  
  <script setup>

  import {useRandomColorPicker} from '../composables/ColorPicker'
  const { colors, message, matchColor } = useRandomColorPicker()
  </script>
  
  <style></style>