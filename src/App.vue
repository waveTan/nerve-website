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
    width: 100%;
    background-size: 100% 100%;
  }

  .home-bg {
    height: 6200px;
    background: #ffffff url("./assets/img/home-bg.png") repeat-y;

  }

  .bg {
    height: 4260px;
    background: #ffffff url("./assets/img/scene-bg.png") repeat-y;
  }

</style>
