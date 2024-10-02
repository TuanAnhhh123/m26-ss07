<template>
    <div>
      <h2>Thêm sản phẩm mới</h2>
      <form @submit.prevent="submitForm">
        <div>
          <label for="productCode">Mã sản phẩm:</label>
          <input type="text" id="productCode" v-model="product.productCode" />
        </div>
        <div>
          <label for="productName">Tên sản phẩm:</label>
          <input type="text" id="productName" v-model="product.productName" />
        </div>
        <div>
          <label for="price">Giá:</label>
          <input type="number" id="price" v-model="product.price" />
        </div>
        <div>
          <label for="quantity">Số lượng:</label>
          <input type="number" id="quantity" v-model="product.quantity" />
        </div>
        <button type="submit">Thêm mới</button>
      </form>
    </div>
  </template>
  
  <script>
  export default {
    data() {
      return {
        product: {
          productCode: '',
          productName: '',
          price: null,
          quantity: null
        }
      };
    },
    methods: {
      submitForm() {
        console.log(this.product);

      }
    }
  };
  </script>
  
  <style scoped>
  </style>
  