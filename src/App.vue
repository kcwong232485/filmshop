<template>
  <Header />   
  <Section />
  <Footer />
</template>

<script>
//import Card from './components/Card.vue'
import Header from './components/Header.vue'
import Footer from './components/Footer.vue'
import Section from './components/Section.vue'

export default {
  name: 'App',
  components: {
    Header, Footer, Section,
  },
  data() {
    return {
      fruit: "Apple",
    };
  },
  methods: {
    handleClick() {
      console.log(this.$refs.subtitle);
      this.$refs.subtitle.classList.add("custom-class")
    }
  }
};
</script>

<style>
#app {
  font-family: Avenir, Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  text-align: center;
  color: #2c3e50;
  margin-top: 60px;
}
</style>
