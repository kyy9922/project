<template>
  <div id="wrap">
    <div class="inner">
      <header id="header">        
        <nav class="h_menu">
          <h2 class="blind">Menu</h2>
          <button type="button" class="hm_btn">
            <i></i>
            <i></i>
            <ul style="display:none;">
              <li>
                <strong>01</strong>
                <span>About</span>
                <a href="/weare/">WE ARE</a>
              </li>
              <li>
                <strong>02</strong>
                <span>Design</span>
                <a href="/service/">SERVICE</a>
              </li>
              <li>
                <strong>03</strong>
                <span>Develop</span>
                <a href="/work/">WORK</a>
              </li>
              <li>
                <strong>04</strong>
                <span>Map</span>
                <a href="/insight/">INSIGHT</a>
              </li>              
            </ul>    
          </button>
        </nav>
        <div class="h_logo">
          <a href="/"><h1 class="logo"></h1></a>
        </div>
    </header>
    
    <div class="photo_wrap">
      <div class="photo_box">
        <div class="image"></div>               
      </div>      
      <a href="#" class="about">About me</a>   
    </div>
      <div class="slogan">
        <p class="slogan_txt1 font-serif">Kwon D Room</p>
        <p class="slogan_txt2"
          >Publishe, Front-end Developer, Branding, UXUI</p>
        <p class="slogan_txt3">
          <span class="block">디자인 하는 개발자, 개발하는 디자이너 겸손함을 겸비한</span>
          <b>개발 + 디자인</b>을 하는 <b>개자이너 권디</b>입니다.</p>
      </div>
      <div class="scrolldown">
        <p>scroll down</p>
      </div>
      <div class="edge_txt">
        <strong>GAEZINER</strong>
        <span>DESIGN PLUS DEVELOPER</span>
      </div>
    </div>
  </div>
</template>

<script>
export default {
  name: "headerComp",
};
</script>

<style>

</style>