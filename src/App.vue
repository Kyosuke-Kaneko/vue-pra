<template>
  <div id="app">
    <Header @getChildText="showChildText"></Header>
    <p v-for="(item,index) in textList" :key="index">{{item}}</p>
  </div>
</template>

<script>
import Header from "./components/Header";
export default {
  data() {
    return {
      textList: []
    };
  },
  methods: {
    showChildText(childText) {
      this.textList.push(childText);
    }
  },
  components: {
    Header
  }
};
</script>