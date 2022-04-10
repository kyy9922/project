<template> 
    
    <Header />
    <Content />

    
    <footer id="footer">
      <div class="footup">
        <ul>
          <li>
            <strong>TEL</strong>
            <span>010-0000-0000</span>
          </li>
          <li>
            <strong>E-MAIL</strong>
            <span>kyy9922@naver.com</span>
          </li>
          <li>
            <strong>INSTAGRAM</strong>
            <span>@kyw_pr</span>
          </li>
        </ul>
      </div>
      <div class="footdown">
        <p>Publishe, Front-end Developer, Branding, UIUX</p>
        <p>© 2022. Kwon D. All rights reserved.</p>
      </div>
    </footer>
  
</template>

<script>
import Header from './components/Header.vue';
import Content from './components/Content.vue';

export default {
  name: 'App',
  components: {
    Header,Content,
  }
}
</script>

<style>
  @import './assets/css/style.css';
</style>
