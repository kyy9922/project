<template> 
    
    <Header />
    <Content />
    <Footer />

    
    
  
</template>

<script>
import Header from './components/Header.vue';
import Content from './components/Content.vue';
import Footer from './components/Footer.vue';

export default {
  name: 'App',
  data (){
    return{
    }
  },  
  components: {
    Header,Content,Footer,
  },
  mounted() {
  }
}
</script>

<style>
  @import './assets/css/style.css';
</style>
