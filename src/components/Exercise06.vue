<template>
    <div>
      <h2>Chọn sở thích của bạn:</h2>
      <div>
        <input type="checkbox" id="reading" value="Đá bóng" v-model="selectedHobbies" />
        <label for="football">Đá bóng</label>
      </div>
      <div>
        <input type="checkbox" id="traveling" value="Bóng chuyền" v-model="selectedHobbies" />
        <label for="valleyball">Bóng chuyền</label>
      </div>
      <div>
        <input type="checkbox" id="sports" value="code" v-model="selectedHobbies" />
        <label for="code">code</label>
      </div>
      <div>
        <input type="checkbox" id="music" value="Bơi lội" v-model="selectedHobbies" />
        <label for="swim">Bơi lội</label>
      </div>
  
      <h3>Sở thích của bạn:</h3>
      <ul>
        <li v-for="(hobby, index) in selectedHobbies" :key="index">{{ hobby }}</li>
      </ul>
    </div>
  </template>
  
  <script>
  export default {
    data() {
      return {
        selectedHobbies: [] 
      };
    }
  };
  </script>
  
  <style scoped>
  
  </style>
  