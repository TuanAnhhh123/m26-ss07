<template>
    <div>
      <label for="email">Nhập địa chỉ email:</label>
      <input 
        type="email" 
        v-model="email" 
        id="email" 
        placeholder="Nhập email của bạn"
      />
      <p>Email đã nhập: {{ email }}</p>
    </div>
  </template>
  
  <script>
  export default {
    data() {
      return {
        email: ''
      }
    }
  }
  </script>
  
  <style scoped>
  input {
    margin-top: 10px;
    padding: 8px;
    font-size: 16px;
  }
  
  p {
    margin-top: 15px;
    font-size: 18px;
    color: #e3d8d8;
  }
  </style>
  