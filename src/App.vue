<template>
  <div id="app">
    <video autoplay="autoplay" muted="muted" loop="loop" id="videobg">
      <source src="http://www.seedland.cc/assets/videos/videobg.mp4" type="video/mp4">
    </video>
    <full-page
      class="fullpage-container"
      ref="fullpage"
      :options="options"
      id="fullpage"
    >
      <div class="section"><HelloWorld/></div>
      <div class="section"><about/></div>
      <div class="section"><development/></div>
      <div class="section"><news/></div>
      <div class="section"><joinus/></div>
      <div class="section"><whistleblower/></div>
      <div class="section"><contact/></div>
    </full-page>
  </div>
</template>

<script type="text/javascript">
import '@/assets/index.css';
import development from '@/components/development.vue';
import HelloWorld from '@/components/HelloWorld.vue';
import about from '@/components/about.vue';
import news from '@/components/news.vue';
import joinus from '@/components/joinus.vue';
import whistleblower from '@/components/whistleblower.vue';
import contact from '@/components/contact.vue';
export default {
  data() {
    return {
      options: {
        licenseKey: "4F375E3E-7D814D7F-B82954BA-31DC667F",
        menu: "#menu",
        anchors: [
          "landing",
          "about",
          "development",
          "news",
          "joinus",
          "whistleblower",
          "contact",
        ],
        sectionsColor: [
        ]
      },
    };
  },
  components: {
    development,
    HelloWorld,
    about,
    news,
    joinus,
    whistleblower,
    contact,
  }
};
</script>

<style lang="less">
.simplebar-scrollbar:before {
    position: absolute;
    content: '';
    background: #fff !important;
    border-radius: 7px;
    left: 0;
    right: 0;
    opacity: 0;
    -webkit-transition: opacity .2s linear;
    transition: opacity .2s linear;
}
::-webkit-scrollbar {
  width: 4px;
  background-color: #7c849271;
  border-radius: 20px;
}
::-webkit-scrollbar-thumb {
  background-color: white;
  border-radius: 20px;
}
::-webkit-scrollbar-thumb:hover {
  background-color: white;
}
::-webkit-scrollbar-thumb:active {
  border: 0;
  border-radius: 20px;
  background-color:white;
  height: 10px;
}
::-webkit-scrollbar-thumb:window-inactive {
  background-color: white;
}
body html{
  padding: 0;
  margin: 0;
  box-sizing: border-box;
  color: #fff;
}
.swiper-wrapper{
  transition-duration: 0ms;
    transform: translate3d(0px, 0px, 0px);
    display: flex;
    width: 100%;
}
</style>