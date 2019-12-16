<template>
    <simplebar class="deve-box" data-simplebar-auto-hide="trun">
      <div class="flex-cell">
        <div
          class="flex-cell-card"
          v-for="(item, index) in deveDataTop"
          :key="index"
          :style="{ backgroundImage: item.bgUrl }"
        >
          <div class="bg-color"></div>
          <div class="deve-item-title">
            <div class="title-cn">{{ item.titleCn }}</div>
            <div class="title-en">{{ item.titleEn }}</div>
          </div>
          <div class="deve-item-btn">
            <div :class="'btn-push-' + index" v-for="index in 4" :key="index">
              +
            </div>
            <div class="btn-box">EXPLORE</div>
            <div class="box-line-top"></div>
            <div class="box-line-left"></div>
            <div class="box-line-right"></div>
            <div class="box-line-bottom"></div>
          </div>
        </div>
      </div>
      <div class="flex-cell">
        <div
          class="flex-cell-card"
          v-for="(item, index) in deveDatatow"
          :key="index"
          :style="{ backgroundImage: item.bgUrl }"
        >
          <div class="bg-color"></div>
          <div class="deve-item-title">
            <div class="title-cn">{{ item.titleCn }}</div>
            <div class="title-en">{{ item.titleEn }}</div>
          </div>
          <div class="deve-item-btn">
            <div :class="'btn-push-' + index" v-for="index in 4" :key="index">
              +
            </div>
            <div class="btn-box">EXPLORE</div>
            <div class="box-line-top"></div>
            <div class="box-line-left"></div>
            <div class="box-line-right"></div>
            <div class="box-line-bottom"></div>
          </div>
        </div>
      </div>
    </simplebar>
</template>

<script>
import simplebar from "simplebar-vue";
import "simplebar/dist/simplebar.min.css";
export default {
  name: "development",
  components: {
    simplebar
  },
  data() {
    return {
      deveDataTop: [
        {
          bgUrl:
            "url(http://www.seedland.cc/wp/wp-content/uploads/2018/10/广州增城蔷薇国际.jpg)",
          titleCn: "广州蔷薇花园",
          titleEn: "QIANGWEI HUAYUAN"
        },
        {
          bgUrl:
            "url(http://www.seedland.cc/wp/wp-content/uploads/2018/10/广州常春藤-1.jpg)",
          titleCn: "广州常春藤",
          titleEn: "BOSTON IVY"
        },
        {
          bgUrl:
            "url(http://www.seedland.cc/wp/wp-content/uploads/2019/08/3e658b0fa85713ed7a6d47caeb276c6.jpg)",
          titleCn: "永川蔷薇国际",
          titleEn: "ROSA INTERNATIONAL"
        },
        {
          bgUrl:
            "url(http://www.seedland.cc/wp/wp-content/uploads/2018/10/惠州常春藤.jpg)",
          titleCn: "惠州常春藤",
          titleEn: "ROYAL IVY"
        },
        {
          bgUrl:
            "url(http://www.seedland.cc/wp/wp-content/uploads/2018/10/惠州木槿雅著.jpg)",
          titleCn: "惠州木槿雅著",
          titleEn: "RIVER ROSELLE"
        },
        {
          bgUrl:
            "url(http://www.seedland.cc/wp/wp-content/uploads/2019/06/太原紫藤公馆.jpg)",
          titleCn: "太原紫藤公馆",
          titleEn: "THE WISTERIA"
        },
        {
          bgUrl:
            "url(http://www.seedland.cc/wp/wp-content/uploads/2019/06/成都海棠名著.jpg)",
          titleCn: "成都海棠名著",
          titleEn: "BEGONIA WEAVE"
        },
        {
          bgUrl:
            "url(http://www.seedland.cc/wp/wp-content/uploads/2018/10/三亚海棠华著.jpg)",
          titleCn: "三亚海棠华著",
          titleEn: "CRYSTAL BAY"
        },
      ],
      deveDatatow: [
        {
          bgUrl:
            "url(http://www.seedland.cc/wp/wp-content/uploads/2018/10/昆明花鹤翎.jpg)",
          titleCn: "昆明花鹤翎",
          titleEn: "CAMILLIA RISE"
        },
        {
          bgUrl:
            "url(http://www.seedland.cc/wp/wp-content/uploads/2019/06/天津海棠雅著.jpg)",
          titleCn: "天津海棠雅著",
          titleEn: "HOUSE OF BEGONIA"
        },
        {
          bgUrl:
            "url(http://www.seedland.cc/wp/wp-content/uploads/2018/10/深圳剑兰郡.jpg)",
          titleCn: "深圳剑兰郡",
          titleEn: "THE GLADIOLUS"
        },
        {
          bgUrl:
            "url(http://www.seedland.cc/wp/wp-content/uploads/2019/06/遵义蔷薇国际.jpg)",
          titleCn: "遵义蔷薇国际",
          titleEn: "ROSE INTERNATIONAL GARDEN"
        },
        {
          bgUrl:
            "url(http://www.seedland.cc/wp/wp-content/uploads/2018/10/ORCHID-SHORE-Intro-2.jpg)",
          titleCn: "武汉君兰汀岸",
          titleEn: "ORCHID SHORE"
        },
        {
          bgUrl:
            "url(http://www.seedland.cc/wp/wp-content/uploads/2019/06/无锡玫瑰庄园.jpg)",
          titleCn: "无锡玫瑰庄园",
          titleEn: "ROSE MANOR"
        },
        {
          bgUrl:
            "url(http://www.seedland.cc/wp/wp-content/uploads/2019/06/中山璟湖城.jpg)",
          titleCn: "中山璟湖城",
          titleEn: "LAKEVIEW COMMUNITY"
        },
        {
          bgUrl:
            "url(http://www.seedland.cc/wp/wp-content/uploads/2018/10/六盘水紫藤庄园.jpg)",
          titleCn: "六盘水紫藤庄园",
          titleEn: "WISTERIA LAKE"
        }
      ]
    }
  }
}
</script>
<style lang="less">
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
.flex-cell {
  display: block;
  width: 100%;
  position: relative;
  height: 100%;
  white-space: nowrap;
}
.flex-cell-card {
  float: unset;
  display: inline-block;
  position: relative;
  width: 25%;
  box-sizing: border-box;
  height: 50vh;
  background-color: #ddd;
  background-size: cover;
  background-repeat: no-repeat;
}
.bg-color {
  display: block;
  position: absolute;
  width: 100%;
  height: 50vh;
  cursor: pointer;
  transition: all 0.3s;
  background: rgba(0,0,0,0.7);
}
.bg-color:hover{
  background: rgba(0, 0, 0, 0.35);
}
.deve-item-title{
  color: #fff;
  z-index: 1;
  position: relative;
  font-size: 15px;
  display: block;
  margin-left: 20px;
  padding-top: 20px;
  margin-right: 20px;
  .title-cn{
    letter-spacing: 2px;
    font-size: 20px;
  }
  .title-en{
    position: absolute;
    bottom: -25px;
    z-index: 1000;
    letter-spacing: 2px;
    font-size: 14px;
    white-space: pre-line;
  }
}
.deve-item-btn {
  text-align: center;
  position: absolute;
  width: 125px;
  right: 10%;
  top: calc(50vh - 10vh);
  .btn-push-1 {
    color: #fff;
    position: absolute;
    left: -4px;
    bottom: -8px;
    transition: transform 0.7s ease-in-out;
  }
  .btn-push-2 {
    color: #fff;
    position: absolute;
    right: -6px;
    bottom: -8px;
    transition: transform 0.7s ease-in-out;
  }
  .btn-push-3 {
    color: #fff;
    position: absolute;
    left: -5px;
    bottom: -8px;
    z-index: 2 !important;
    transition: transform 0.7s ease-in-out;
  }
  .btn-push-4 {
    color: #fff;
    position: absolute;
    right: -6px;
    bottom: -8px;
    z-index: 2 !important;
    transition: transform 0.7s ease-in-out;
  }
}
.btn-box {
  opacity: 0;
  z-index: 1;
  font-size: 14px;
  margin-top: 22px;
  float: right;
  width: 125px;
  height: 33px;
  padding-top: 6px;
  padding-bottom: 6px;
  color: #fff;
  background-color: rgba(0, 0, 0, 0.5);
  cursor: pointer;
  font-family: "DIN-Regular";
  letter-spacing: 3px;
  border-bottom: 1px solid #ffffff;
  text-align: center;
  line-height: 21px;
  transition: opacity 1.3s ease-in-out;
}
 .box-line-top {
  width: 0px;
  height: 1px;
  background: #fff;
  position: absolute;
  bottom: 33px;
  right: 0;
  transition: width 1.6s;
  opacity: 0.7;
}
.box-line-left {
  width: 1px;
  height: 0px;
  background: #fff;
  position: absolute;
  left: 0px;
  bottom: 0px;
  transition: height 2.3s;
  opacity: 0.7;
}
.box-line-right {
  width: 1px;
  height: 0px;
  background: #fff;
  position: absolute;
  right: 0px;
  top: 21px;
  transition: height 2s;
  opacity: 0.7;
}
.box-line-bottom{
  width: 125px;
  height: 1px;
  background: #fff;
  position: absolute;
  bottom: 0px;
  right: 0;
  opacity: 0.7;
}
.btn-box:hover {
  background-color: rgba(179, 175, 175, 0.397);
}

.flex-cell-card:hover {
  .btn-push-1 {
    transform: rotate(360deg);
  }
  .btn-push-2 {
    transform: rotate(360deg);
  }
  .btn-push-3 {
    transform: translateY(-33px) rotate(360deg);
  }
  .btn-push-4 {
    transform: translateY(-33px) rotate(360deg);
  }
  .btn-box {
    opacity: 1;
  }
  .box-line-top {
    width: 125px;
  }
  .box-line-left {
    height: 33px;
  }
  .box-line-right {
    height: 33px;
  }
}
</style>