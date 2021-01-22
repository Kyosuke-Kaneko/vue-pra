<template>
  <div id="app">
    名前：
    <input type="text" v-model="name" />
    値段：
    <input type="number" v-model="price" />
    <button @click="add">果物</button>
     <ul>
      <li v-for="(item,index) in list" :key="index">{{ item.name }}は{{ item.price }}円</li>
    </ul>
  </div>
</template>

<script>
export default {
  data() {
    return {
      name: "",
      price: 0,
      list: [
        { name: "りんご", price: 200 },
        { name: "オレンジ", price: 100 },
        { name: "バナナ", price: 500 }
      ]
    };
  },
  methods: {
    add() {
      this.list.push({
        name: this.name,
        price: this.price
      });
    }
  }
};
</script>