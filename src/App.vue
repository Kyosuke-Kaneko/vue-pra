<template>
  <div id="app">
    <table>
      <tr>
        <th>名前</th>
        <th>値段</th>
        <th>個数</th>
      </tr>
      <tr>
        <td>{{pencil.name}}</td>
        <td>{{pencil.price}}</td>
        <td>{{pencil.quantity}}</td>
      </tr>
      <tr>
        <td>{{eraser.name}}</td>
        <td>{{eraser.price}}</td>
        <td>{{eraser.quantity}}</td>
      </tr>
      <tr>
        <td>{{notebook.name}}</td>
        <td>{{notebook.price}}</td>
        <td>{{notebook.quantity}}</td>
      </tr>
    </table>
  </div>
</template>

<script>
export default {
  data() {
    return {
      pencil:{
        name: "鉛筆",
        price: 100,
        quantity: 0
      },
      eraser:{
        name:'消しゴム',
        price:150,
        quantity:0
      },
      notebook:{
        name:'ノート',
        price:200,
        quantity:0
      }
    };
  }
};
</script>
<style>
th {
  width: 30%;
  background: #e6e6e6;
}
td {
  width: 30%;
  background: #f2f2f2;
}
</style>