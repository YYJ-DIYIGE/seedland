<template>
<div class="HelloWorld">
  <div class="lateralNav">
     <img src="@/assets/hamburger.png" @click="navLock = true" >
  </div>
  <div class="navbar home">
      <div class="navbar-left">
        <img src="@/assets/Logo_Anim.gif">
      </div>
        <div class="menu">
          <a class="menu-item" data-menuanchor="about" href="#about">关于实地</a>
          <a class="menu-item" data-menuanchor="development" href="#development">地产开发</a>
          <a class="menu-item" data-menuanchor="news" href="#news">最新消息</a>
          <a class="menu-item" data-menuanchor="joinus" href="#joinus">加入实地</a>
          <a class="menu-item" data-menuanchor="whistleblower" href="#whistleblower">廉洁举报</a>
          <a class="menu-item" data-menuanchor="contact" href="#contact">联系我们</a>
        </div>
  </div>
  <div class="landing-grid">
    <div class="landing-Hgrid-box-center">
      <div :class="['landing-Hgrid-c'+ index ,'landing-grid-horizontal', 'runcenterline']" v-for="index in 2" :key="index"></div>
    </div> 
    <div class="landing-Hgrid-box">
      <div :class="['landing-Hgrid-' + index , 'landing-grid-horizontal', 'runh'+ index]" v-for="index in 3" :key="index"></div> 
    </div> 
    <div class="landing-Vgrid-box">
      <div :class="['landing-Vgrid-' + index, 'landing-grid-vertical', 'runv'+ index]" v-for="index in 7" :key="index"></div>
    </div>
  </div>
  <div class="landing-cross-box">
    <p :class="'landing-cross' + index" v-for="index in 17" :key="index">+</p>
  </div>
  <div class="landing-boby">
    <div class="landing-content">
      <div class="landing-title">THE FUTURE</div>
      <div class="landing-title">IS HERE</div>
      <div class="landing-subTitle">未来•就在眼前</div>
    </div>
    <div class="landing-mousescroll">
      <div class="landing-mousescrolltextcn">向下滚动</div>
      <div class="landing-mousescrolltexten">Scroll down for more</div>
      <span class="landing-scroll-btn">
        <span class="landing-mouse">
          <span></span>
        </span>
      </span>
    </div>
  </div>
  <hide v-if="navLock" @close="closeNav" />
</div>
</template>
<script type="text/javascript">
  import hide from "@/components/hide.vue";
  export default{
    name: "HelloWorld",
    components: {
     hide
    },
    data(){
      return{
        navLock: false,
        navbar:[
        {title:'关于实地'},
        {title:'地产开发'},
        {title:'最新消息'},
        {title:'加入实地'},
        {title:'廉洁举报'},
        {title:'联系我们'}
        ]
      } 
    },
  methods: {
    closeNav(val) {
      this.navLock = val;
    }
  },
  }
</script>