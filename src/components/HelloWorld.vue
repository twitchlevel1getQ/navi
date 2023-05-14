<template>
  <div class="bg">
    <div class="logo-img"></div>
    <div class="containerbox">
      <div class="rgpage-box">
        <div class="rgpage-img"></div>
        <div class="rgpage-font">掛號查詢</div>
      </div>
      <div class="rgpage-box2">
        <div class="box2-img"></div>
        <div class="rgpage-font">門診掛號</div>
      </div>
    </div>
    <div class="containerbox">
      <div class="rgpage-box3">
        <div class="box3-img"></div>
        <div class="box3-font">慢籤領藥</div>
      </div>
      <div class="rgpage-box4">
        <div class="box4-img"></div>
        <div class="rgpage-font">看診進度</div>
      </div>
      <div class="rgpage-box5">
        <div class="box5-img"></div>
        <div class="rgpage-font">該看哪科</div>
      </div>
    </div>
  </div>
</template>
<script>
// import VueTouch from 'vue2-touch-events'

export default {
  mounted() {
    this.$store.dispatch("updateArea", 1);
  },
  methods: {
    changelanguage(lang) {
      this.$store.dispatch("updlanguage", lang);
    },
    touchHandler() {
      alert("touchHandler");
    },
    swipeHandler(msg) {},
    goback() {
      this.$router.back();
    },
    jumpPage(src) {
      this.$router.push({
        path: src,
      });
    },
  },
};
</script>
<style scoped>
.logo-img {
  /* Layout Properties */
  position: relative;
  top: 30px;
  left: 80px;
  width: 620px;
  height: 130px;
  /* UI Properties */
  background: transparent url("../../public/images/logo.svg") 0% 0% no-repeat
    padding-box;
  opacity: 1;
}

.rgpage-box3 {
  /* Layout Properties */
  justify-content: flex-start; /* 将 justify-content 设置为 flex-start */
  margin-left: 16px; /* 將 margin-left 設置為 0 */
  display: flex;
  align-items: center;
  position: relative;
  top: 120px;
  left: 60px;
  width: 240px;
  height: 240px;
  /* UI Properties */
  background: transparent linear-gradient(135deg, #d66081 0%, #af2b4f 100%) 0%
    0% no-repeat padding-box;
  box-shadow: 0px 3px 6px #00000029;
  border-radius: 8px;
  opacity: 1;
}
.rgpage-box2 {
  /* Layout Properties */
  justify-content: flex-start; /* 将 justify-content 设置为 flex-start */
  margin-left: 16px; /* 將 margin-left 設置為 0 */
  display: flex;
  align-items: center;
  position: relative;
  top: 90px;
  left: 96px;
  width: 492px;
  height: 240px;
  /* UI Properties */
  background: transparent linear-gradient(134deg, #eaa74c 0%, #ce7d36 100%) 0%
    0% no-repeat padding-box;
  box-shadow: 0px 0px 15px #2c5e4b;
  border-radius: 8px;
  opacity: 1;
}
.rgpage-box {
  /* Layout Properties */
  justify-content: flex-start; /* 将 justify-content 设置为 flex-start */
  margin-right: 0; /* 將 margin-right 設置為 0 */
  display: flex;
  align-items: center;
  position: relative;
  top: 90px;
  left: 80px;
  width: 492px;
  height: 240px;
  /* UI Properties */
  background: transparent linear-gradient(134deg, #60bfc1 0%, #379698 100%) 0%
    0% no-repeat padding-box;
  box-shadow: 0px 0px 15px #2c5e4b;
  border-radius: 8px;
  opacity: 1;
}
.rgpage-img {
  top: 0px;
  left: 24px;
  width: 180px;
  height: 180px;
  background: transparent url("../../public/images/icon-掛號查詢.svg") 0% 0%
    no-repeat padding-box;
  opacity: 1;
  margin-right: 20px;
}
.box2-img {
  top: 0px;
  left: 24px;
  width: 180px;
  height: 180px;
  background: transparent url("../../public/images/icon-門診掛號.svg") 0% 0%
    no-repeat padding-box;
  opacity: 1;
  margin-right: 20px;
}
.box3-img {
  top: 0px;
  left: 24px;
  width: 110px;
  height: 110px;
  background: transparent url("../../public/images/icon-慢箋領藥.svg") 0% 0%
    no-repeat padding-box;
  opacity: 1;
  margin-right: 20px;
}
.box3-font {
  font: var(--unnamed-font-style-normal) normal var(--unnamed-font-weight-bold)
    var(--unnamed-font-size-38) / var(--unnamed-line-spacing-43)
    var(--unnamed-font-family-arial);
  letter-spacing: var(--unnamed-character-spacing-1-14);
  color: var(--unnamed-color-ffffff);
  text-align: center;
  font: normal normal bold 38px/43px Arial;
  letter-spacing: 1.14px;
  color: #ffffff;
  text-shadow: 0px 3px 6px #00000029;
  opacity: 1;
}
.box4-img {
  top: 0px;
  left: 24px;
  width: 180px;
  height: 180px;
  background: transparent url("../../public/images/icon-看診進度.svg") 0% 0%
    no-repeat padding-box;
  opacity: 1;
  margin-right: 20px;
}
.box5-img {
  top: 0px;
  left: 24px;
  width: 180px;
  height: 180px;
  background: transparent url("../../public/images/icon-該看哪科.svg") 0% 0%
    no-repeat padding-box;
  opacity: 1;
  margin-right: 20px;
}
.rgpage-font {
  /* Layout Properties */
  top: 10px;
  left: 20px;
  width: 250px;
  height: 77px;
  padding: 2px 2px 2px;
  /* UI Properties */
  font: var(--unnamed-font-style-normal) normal var(--unnamed-font-weight-bold)
    55px/64px var(--unnamed-font-family-arial);
  color: var(--unnamed-color-ffffff);
  text-align: center;
  font: normal normal bold 55px/64px Arial;
  letter-spacing: 1.65px;
  color: #ffffff;
  text-shadow: 0px 3px 6px #00000029;
  opacity: 1;
}
.rgpage-img,
.box2-img,
.rgpage-font {
  flex: 0 0 auto;
  position: relative;
}

.rgpage-box {
  flex: 1; /* 兩個子元素平均佔據可用空間 */
}

.containerbox {
  display: flex; /* 將容器設置為彈性盒子 */
  flex-direction: row;
  /* width: 55%; */
  width: 1000px;
}
.box {
  flex: 1; /* 兩個子元素平均佔據可用空間 */
  height: 100px;
  background-color: gray;
}
.bg {
  min-width: 1920px;
  min-height: 1080px;
  background: transparent url("../../public/images/bg-03.png") 0% 0% no-repeat
    padding-box;
  opacity: 1;
  width: 100vw;
  height: 100vh;
  position: relative;
}
.bg::before {
  content: "";
  position: absolute;
  top: 0;
  left: 0;
  right: 0;
  bottom: 0;
  background-image: url("../../public/images/bg-03.png") 0% 0% no-repeat
    padding-box;
  background-size: cover;
  background-repeat: no-repeat;
  background-position: center;
}
.body {
  margin-left: 0%;
}
/* CSS重置 */
* {
  margin: 0;
  padding: 0;
  box-sizing: border-box;
  /* 其他重置样式 */
}
</style>
