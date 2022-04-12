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
          <li>
            <div class="pie-chart pie-chart1" title="HTML">
              <span class="center" title="HTML"></span>
            </div>
          </li>
          <li><div class="pie-chart pie-chart2" title="CSS">
              <span class="center" title="CSS"></span>
            </div>
          </li>
          <li><div class="pie-chart pie-chart3" title="JAVASCRIPT">
              <span class="center" title="JAVASCRIPT"></span>
            </div>
          </li>
          <li><div class="pie-chart pie-chart4" title="JQUERY">
              <span class="center" title="JQUERY"></span>
            </div>
          </li>
          <li><div class="pie-chart pie-chart5" title="VUE.JS">
              <span class="center" title="VUE.JS"></span>
            </div>
          </li>
        </ul>
      </div>

      <div class="tab_box">
        <div class="tabs">
          <ul class="tab-menu">
            <li
              v-for="(item, i) in tabs"
              :key="i"
              :v-bind:class="{ active: currentTab === i }"
            >
              <a href="" @click.prevent="currentTab = i">{{ item }}</a>
            </li>
          </ul>
        </div>
        <div class="tab-content">
          <div v-show="currentTab == 0">
            <div class="txt-box">
              <h3 class="font-serif">My All Skill is01</h3>
              <p>
                <span class="block">HTML, CSS, Javascript, Jquery, Vue.js</span>
                Photoshop, illustrator, XD, Figma
              </p>
            </div>
          </div>
          <div v-show="currentTab == 1">
            <div class="txt-box">
              <h3 class="font-serif">My All Skill is02</h3>
              <p>
                <span class="block">HTML, CSS, Javascript, Jquery, Vue.js</span>
                Photoshop, illustrator, XD, Figma
              </p>
            </div>
          </div>
          <div v-show="currentTab == 2">
            <div class="txt-box">
              <h3 class="font-serif">My All Skill is03</h3>
              <p>
                <span class="block">HTML, CSS, Javascript, Jquery, Vue.js</span>
                Photoshop, illustrator, XD, Figma
              </p>
            </div>
          </div>
          <div v-show="currentTab == 3">
            <div class="txt-box">
              <h3 class="font-serif">My All Skill is04</h3>
              <p>
                <span class="block">HTML, CSS, Javascript, Jquery, Vue.js</span>
                Photoshop, illustrator, XD, Figma
              </p>
            </div>
          </div>
        </div>
      </div>

      <div class="slide_box">
        <span class="bk"></span>
        <section class="visual">
          <div>
            <img
              src="https://cdn.pixabay.com/photo/2022/02/23/18/08/kingfisher-7031148_960_720.jpg"
            />
          </div>
          <div>
            <img
              src="https://cdn.pixabay.com/photo/2022/02/20/09/46/lama-7024125_640.jpg"
            />
          </div>
          <div>
            <img
              src="https://cdn.pixabay.com/photo/2019/03/05/05/45/man-4035612_640.jpg"
            />
          </div>
        </section>

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
          <li>
            <div class="pie-chart pie-chart6" title="PHOTOSHOP">
              <span class="center" title="PHOTOSHOP"></span>
            </div>
          </li>
          <li>
            <div class="pie-chart pie-chart7" title="ALLLUSTRATOR">
              <span class="center" title="ALLLUSTRATOR"></span>
            </div>
          </li>
          <li>
            <div class="pie-chart pie-chart8" title="XD">
              <span class="center" title="XD"></span>
            </div>
          </li>
          <li>
            <div class="pie-chart pie-chart9" title="FIGMA">
              <span class="center" title="FIGMA"></span>
            </div>
          </li>
        </ul>
      </div>
    </div>
  </div>
</template>

<script>
export default {
  name: "ContentComp",
  data() {
    return {
      currentTab: 0,
      tabs: ["Tab01", "Tab02", "Tab03", "Tab04"],
    };
  },
  mounted() {
    $(".visual").slick();
    $('.develops_box ul li').eq(0).click(function () {
      draw(90, ".pie-chart1", "#e44d26")
    });
    $('.develops_box ul li').eq(1).click(function () {      
      draw(75, ".pie-chart2", "#1572b6")      
    });
    $('.develops_box ul li').eq(2).click(function () {      
      draw(40, ".pie-chart3", "#e4a126")
    });
    $('.develops_box ul li').eq(3).click(function () {      
      draw(50, ".pie-chart4", "#0868ac")
    });
    $('.develops_box ul li').eq(4).click(function () {      
      draw(45, ".pie-chart5", "#41b883")
    });
    $('.design_box ul li').eq(0).click(function () {     
      draw(90, ".pie-chart6", "#58c7f5");
    });
    $('.design_box ul li').eq(1).click(function () {     
      draw(80, ".pie-chart7", "#ff8c00");
    });
    $('.design_box ul li').eq(2).click(function () { 
      draw(50, ".pie-chart8", "#ff1bc3");
    });
    $('.design_box ul li').eq(3).click(function () {
      draw(50, ".pie-chart9", "#f24e1e");
    });

    function draw(max, classname, colorname) {
      var i = 1;
      var func1 = setInterval(function () {
        if (i < max) {
          color1(i, classname, colorname);
          i++;
        } else {
          clearInterval(func1);
        }
      }, 10);
    }
    function color1(i, classname, colorname) {
      $(classname).css({
        background:
          "conic-gradient(" +
          colorname +
          " 0% " +
          i +
          "%, #cccccc " +
          i +
          "% 100%)",
      });
    }

  },
};
</script>

<style>
</style>