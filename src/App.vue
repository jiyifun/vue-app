<template>
  <div id="wrapper">
    <div class="main">
      <router-view class="main-wrapper" transition="fade" transition-mode="out-in"></router-view>
    </div>
    <vfooter class="footer"></vfooter>
  </div>

</template>

<script type="text/babel">
  import Vfooter from './components/Vfooter'
  import store from './vuex/store'

  export default {
    components: {
      Vfooter
    },
    store
  }
</script>

<style>
@import '/style/css/variable';
  body {
    -webkit-font-smoothing:antialiased;
    margin: 0;
    padding: 0;
    font-family: -apple-system, "Helvetica Neue", Arial, "PingFang SC", "Hiragino Sans GB", STHeiti, "Microsoft YaHei", "Microsoft JhengHei", "Source Han Sans SC", "Noto Sans CJK SC", "Source Han Sans CN", "Noto Sans SC", "Source Han Sans TC", "Noto Sans CJK TC", "WenQuanYi Micro Hei", SimSun, sans-serif;
    color: #404040;
    line-height: 1.7;
    height:100%;
  }
  #wrapper {
    position: absolute;
    top: 0;
    left: 0;
    right: 0;
    bottom: 0;
  }
 .main {
  position: absolute;
  top: 0;
  left: 0;
  right: 0;
  bottom: 100px;
 }
 .footer {
  position: absolute;
  height: 100px;
  left: 0;
  right: 0;
  bottom: 0;
  border-top: 2px solid $bordercolor;
 }
</style>
