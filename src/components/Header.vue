<template>
  <div id="wrap">
    <div class="inner">
      <header id="header">        
        <nav class="h_menu">
          <button type="button" class="hm_btn">
            <i></i>
            <i></i>
            <span class="blind">전체메뉴</span>
          </button>
          <div class="hm_wrap">
            <ul>
              <li>
                <strong>01</strong>
                <a href="#">ABOUT ME</a>
              </li>
              <li>
                <strong>02</strong>
                <a href="#">PORTFOLIO</a>
              </li>
              <li>
                <strong>02</strong>
                <a href="#">MY ALL SKILL</a>
              </li>              
            </ul>
          </div>
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
  mounted() {
    /* 메뉴 오픈 */
	$(document).on('click', '.hm_btn', function(){
		$('.h_menu').stop().toggleClass('open')
    $('.hm_btn').toggleClass('changed').stop();
    $('.hm_btn i').toggleClass('changed').stop();
	});
  
	$(document).on("click", '.ff_btn', function(){
		$('.f_family').stop().toggleClass('on');
		$(".check .csft_list.t1").removeClass('open');
		$(".check .csft_list.t2").removeClass('open');
	});
    

  },
}



</script>

<style>

</style>