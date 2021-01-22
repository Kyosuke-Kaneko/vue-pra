<template>
  <div id="app">
    <p>合計金額:{{ price }}(税抜)</p>
    <p>合計金額:{{ includeTax }}(税込)</p>
  </div>
</template>

<script>
export default {
  data() {
    return {
      price: 300
    };
  },
  computed: {
    includeTax() {
      return this.price * 1.1
    }
  }
};
</script>