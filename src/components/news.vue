<template>
  <div class="news">
   <div class="lateralNav">
        <img src="@/assets/hamburger.png" @click="navLock = true" >
    </div>
    <div class="news-content">
      <div class="news-secondary-title">最新消息</div>
      <div class="news-main-title">LATEST NEWS</div>
    </div>
    <footer class="footer-btn">
      <div class="footer-container">
        <div class="btn-left">
          <p>找到更多</p>
          <span>了解更多</span>
        </div>
        <div class="btn-right">
          <div class="arrow"></div>
          <div class="point"></div>
        </div>
        <div :class="'plus' + item" v-for="(item,index) in 4" :key="index">+</div>
      </div>
    </footer>
    <hide v-if="navLock" @close="closeNav" />
  </div>
</template>
<script type="text/javascript">
  import hide from "@/components/hide.vue";
  export default{
    name: "news",
    components: {
    hide
    },
    data(){
      return{
        navLock:false
      }
    },
    methods: {
    closeNav(val) {
      this.navLock = val;
    }
  },
  }
</script>
<style lang="less">

</style>