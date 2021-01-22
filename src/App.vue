<template>
  <div id="app">
    <input type="text" :value="message" />
  </div>
</template>

<script>
export default {
  data() {
    return {
      message: "Hello"
    };
  }
};
</script>