<template>
  <div id="app" class="app" :class="bgChoice">
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
        bgChoice: 'home-bg',
      };
    },
    components: {
      HeaderBar,
      BottomBar
    },
    watch: {
      $route(to) {
        if (to.path === '/home' || this.$route.path === '/') {
          this.bgChoice = 'home-bg'
        } else if (to.path === '/team') {
          this.bgChoice = 'team-bg'
        } else {
          this.bgChoice = 'bg'
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
        if (this.$route.path === '/home' || this.$route.path === '/') {
          this.bgChoice = 'home-bg'
        } else if (this.$route.path === '/team') {
          this.bgChoice = 'team-bg'
        } else {
          this.bgChoice = 'bg'
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

  .team-bg {
    min-height: 1752px;
    background: #ffffff url("./assets/img/team-bg.png") repeat-y;
  }

  .bg {
    height: 4260px;
    background: #ffffff url("./assets/img/scene-bg.png") repeat-y;
  }

</style>
