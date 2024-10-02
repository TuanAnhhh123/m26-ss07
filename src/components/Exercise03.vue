<template>
    <div>
      <h2>Nhập ngày sinh của bạn:</h2>
      <input type="date" v-model="birthDate" />
      <p>Ngày sinh được chọn: <strong>{{ formattedDate }}</strong></p>
    </div>
  </template>
  
  <script>
  export default {
    data() {
      return {
        birthDate: null 
      };
    },
    computed: {
      formattedDate() {
   
        if (this.birthDate) {
          const options = { year: 'numeric', month: '2-digit', day: '2-digit' };
          return new Date(this.birthDate).toLocaleDateString('vi-VN', options);
        }
        return ''; 
      }
    }
  };
  </script>
  
  <style scoped>

  </style>
  