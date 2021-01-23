<template>
  <div class="home">
    <Header @getChildText="showChildText"></Header>
    <SideMenu></SideMenu>
    <Footer></Footer>
    <p>{{text}}</p>
  </div>
</template>

<script>
import Header from "./components/Header";
import SideMenu from './components/SideMenu.vue';
import Footer from './components/Footer.vue';
export default {
  data() {
    return {
      text: "",
    };
  },
  methods: {
    showChildText(childText) {
      this.text = childText;
    }
  },
  components: {
    Header,
    SideMenu,
    Footer,
  }
};
</script>