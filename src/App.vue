<template>
  <div id="app" class="app" :class="bgChoice ? 'home-bg': 'bg'">
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
    data() {
      return {
        bgChoice: true,
      };
    },
    components: {
      HeaderBar,
      BottomBar
    },
    watch: {
      $route(to) {
        if (to.path === '/home' || to.path === '/') {
          this.bgChoice = true
        } else {
          this.bgChoice = false
        }
      }
    },
    created() {
      this.getPath();
    },
    mounted() {
    },
    methods: {

      /**
       * @disc: 路由变化
       * @date: 2019-11-08 10:06
       * @author: Wave
       */
      getPath() {
        if (this.$route.path === '/home' || to.path === '/') {
          this.bgChoice = true
        } else {
          this.bgChoice = false
        }
      }

    }
  }
</script>

<style lang="less">
  @import "assets/css/base.less";

  .app {
    min-width: 1520px;
    background-size: 100% 100%;
    @media screen and (min-width: 1024px) {
      min-width: 1024px;
    }
    @media screen and (min-width: 1360px) {
      min-width: 1200px;
    }
    @media screen and (min-width: 1600px) {
      min-width: 1520px;
    }
  }

  .home-bg {
    min-height: 5500px;
    background: #ffffff url("./assets/img/home-bg.png") repeat-y;
  }

  .bg {
    height: 4260px;
    background: #ffffff url("./assets/img/scene-bg.png") repeat-y;
  }

</style>
