<template>
  <div id="app" class="app">
    <!--<div class="bg1"></div>-->
    <!--<div class="bg2"></div>-->
    <HeaderBar>
    </HeaderBar>
    <router-view>
    </router-view>
    <BottomBar>
    </BottomBar>
  </div>
</template>
<script>
  import HeaderBar from './components/HeaderBar'
  import BottomBar from './components/BottomBar'

  export default {
    components: {
      HeaderBar,
      BottomBar
    },
    methods: {}
  }
</script>

<style lang="less">
  @import "assets/css/base.less";

  .app {
    .bg1 {
      width: 1400px;
      height: 1600px;
      border-radius: 50px;
      background-color: #1a56a4;
      border: 1px solid darkgoldenrod;
      z-index: 1;
      position: absolute;
      right: 0;
      -webkit-transform: rotate(300deg);
      margin: -1100px 50px 0 0;
    }
    .bg2 {
      width: 800px;
      height: 1000px;
      border-radius: 50px;
      background-color: #f6f9fe;
      border: 1px solid red;
      z-index: 1;
      position: absolute;
      -webkit-transform: rotate(340deg);
      margin: 350px 0 0 0;
    }
  }
</style>
