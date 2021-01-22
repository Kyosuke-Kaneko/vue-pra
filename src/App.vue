<template>
  <div id="app">
    <p @click="change">{{text}}</p>
  </div>
</template>

<script>
export default {
  data() {
    return {
      text:"クリックする前のテキスト" 
    };
  },
  methods: {
    change() {
      this.text = "クリックしたあとのテキスト";
    }
  }
};
</script>