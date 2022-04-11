<template> 
    
    <Header />
    <Content />
    <Footer />
    
  
</template>

<script>
import Header from './components/Header.vue';
import Content from './components/Content.vue';
import Footer from './components/Footer.vue';
import $ from 'jquery';

export default {
  name: 'App',
  components: {
    Header,Content,Footer,
  }
}
</script>

<style>
  @import './assets/css/style.css';
</style>
