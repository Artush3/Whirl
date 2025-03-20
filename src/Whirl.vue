<script>
import Header from './components/Header.vue';
import Main from './components/Main/Main.vue';
import Footer from './components/Footer.vue';
export default {
  name: "Whirl",
  mounted() {
    document.title = "Home"
  },
  components: { Header, Main, Footer }
}
</script>

<template>
  <Header></Header>
  <Main></Main>
  <Footer></Footer>
</template>