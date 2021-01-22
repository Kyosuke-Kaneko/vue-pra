<template>
  <div id="app">
    <table>
      <tr v-for="(data,index) in Vegetables" :key="index">
        <th>{{index}}</th>
        <td>{{data.name}}</td>
        <td>{{data.price}}円</td>
      </tr>
    </table>
  </div>
</template>

<script>
export default {
  data() {
    return {
      Vegetables: [
        { name: "じゃがいも", price: 300 },
        { name: "イチゴ", price: 400 },
        { name: "カボチャ", price: 500 }
      ]
    };
  }
};
</script>