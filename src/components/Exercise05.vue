<template>
    <div>
      <h2>Chọn giới tính của bạn:</h2>
      <div>
        <input type="radio" id="male" value="Nam" v-model="selectedGender" />
        <label for="male">Nam</label>
      </div>
      <div>
        <input type="radio" id="female" value="Nữ" v-model="selectedGender" />
        <label for="female">Nữ</label>
      </div>
      <div>
        <input type="radio" id="other" value="Khác" v-model="selectedGender" />
        <label for="other">Khác</label>
      </div>
  
      <p>Giới tính đã chọn: <strong>{{ selectedGender }}</strong></p>
    </div>
  </template>
  
  <script>
  export default {
    data() {
      return {
        selectedGender: '' 
      };
    }
  };
  </script>
  
  <style scoped>
 
  </style>
  