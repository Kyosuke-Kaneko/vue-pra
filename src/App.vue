<template>
  <div id="app">
    <ul v-for="(data,index) in list" :key="index">
    <li>{{index}}:{{data.name}}は{{data.price}}円です</li>
    <li v-if="data.price > 300">高いです</li>
    </ul>
  </div>
</template>

<script>
export default {
  data() {
    return {
      list: [
        { name: "りんご", price: 200 },
        { name: "オレンジ", price: 100 },
        { name: "バナナ", price: 500 }
      ]
    };
  },
  methods: {


  }
};
</script>