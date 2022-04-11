<template>
  <div id="content">
    <div class="myportfolio">
      <div>
        <h3 class="title_h3 font-serif">
          <span class="block font-serif">My</span>Portfolio
        </h3>
      </div>
      <div>
        <div class="tit-box">
          <h4 class="title_h4 font-serif">UIUX Design</h4>
          <a href="#" class="more">Detail view</a>
        </div>
      </div>
      <div>
        <div class="tit-box">
          <h4 class="title_h4 font-serif">Front end Develop</h4>
          <a href="#" class="more">Detail view</a>
        </div>
      </div>
    </div>

    <div class="skill">
      <div class="develops_box">
        <h4 class="title_h4 font-serif">Front end Develop Skill</h4>
        <ul>
          <li>HTML</li>
          <li>CSS</li>
          <li>JS</li>
          <li>JQUERY</li>
          <li>VUE</li>
        </ul>
      </div>

      <div class="tab_box">
        <div class="tabs">
          <ul class="tab-menu">
            <li v-for="(item,i) in tabs" :key="i" :v-bind:class="{active:currentTab === i}">
              <a href="" @click.prevent="currentTab = i">{{item}}</a>
            </li>
          </ul>
        </div>
        <div class="tab-content">
          <div v-show="currentTab == 0">
            <div class="txt-box">
              <h3 class="font-serif">My All Skill is</h3>
              <p>
                <span class="block">HTML, CSS, Javascript, Jquery, Vue.js</span>
                Photoshop, illustrator, XD, Figma
              </p>
            </div>
          </div>
          <div v-show="currentTab == 1">
            <div class="txt-box">
              <h3 class="font-serif">My All Skill is2</h3>
              <p>
                <span class="block">HTML, CSS, Javascript, Jquery, Vue.js</span>
                Photoshop, illustrator, XD, Figma
              </p>
            </div>
          </div>
          <div v-show="currentTab == 2">
            <div class="txt-box">
              <h3 class="font-serif">My All Skill is3</h3>
              <p>
                <span class="block">HTML, CSS, Javascript, Jquery, Vue.js</span>
                Photoshop, illustrator, XD, Figma
              </p>
            </div>
          </div>
          <div v-show="currentTab == 3">
            <div class="txt-box">
              <h3 class="font-serif">My All Skill is4</h3>
              <p>
                <span class="block">HTML, CSS, Javascript, Jquery, Vue.js</span>
                Photoshop, illustrator, XD, Figma
              </p>
            </div>
          </div>
        </div>
        
      </div>

      <div class="slide_box">        

        <div class="custom1">
          <div class="item"><img src="https://cdn.pixabay.com/photo/2022/02/23/18/08/kingfisher-7031148_960_720.jpg"></div>
        </div>
        
        <div class="txt-box">
          <h3 class="font-serif">My mind is</h3>
          <p>
            <span class="block">Design in detail like development</span> As
            emotionally as designing development
          </p>
        </div>
      
      </div>
      <div class="design_box">
        <h4 class="title_h4 font-serif">UI UX Design Skill</h4>
        <ul>
          <li>photoshop</li>
          <li>ai</li>
          <li>xd</li>
          <li>figma</li>
        </ul>
      </div>
    </div>
  </div>
</template>

<script>
export default {
  name: "ContentComp",
  data() {
    return{
      currentTab : 0,
      tabs : ['Tab01','Tab02','Tab03','Tab04']
    }
  },
  computed: {
    
  },
  component : {
    
  },
  mounted() {
    $('.custom1').owlCarousel({
      animateOut: 'slideOutDown',
      animateIn: 'flipInX',
      items:1,
      margin:30,
      stagePadding:30,
      smartSpeed:450
    });
  },
};
</script>

<style>
</style>