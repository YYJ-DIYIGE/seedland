<template>
  <div class="news">
    <div class="lateralNav">
      <img src="@/assets/hamburger.png" @click="navLock = true" >
    </div>
    <div class="news-content joinus-content">
      <div class="news-secondary-title">加入我们</div>
      <div class="news-main-title">joinus</div>
    </div>
    <footer class="footer-btn joinus-footer">
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
    name: "joinus",
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
    }
  }
</script>
<style lang="less">

</style>