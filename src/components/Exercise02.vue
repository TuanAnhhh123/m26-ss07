<template>
    <div>
      <h2>Chọn màu sắc:</h2>
      <input type="color" v-model="selectedColor" />
      <p>Mã màu được chọn: <strong>{{ selectedColor }}</strong></p>
      <div :style="{ backgroundColor: selectedColor }" class="color-preview"></div>
    </div>
  </template>
  
  <script>
  export default {
    data() {
      return {
        selectedColor: '#000000' // Màu mặc định
      };
    }
  };
  </script>
  
  <style scoped>
  .color-preview {
    width: 100px;
    height: 100px;
    margin-top: 10px;
    border: 1px solid #ccc;
  }
  </style>
  