<template>
  <div class="flex flex-col h-screen">
    <Header></Header>
    <Home></Home>
    <Footer></Footer>
  </div>
</template>

<script>
import Home from "./components/Home.vue";
import Footer from "./components/Footer.vue";
import Header from "./components/Header.vue"
export default {
  components: {
    Home,
    Footer,
    Header
  },
};
</script>
