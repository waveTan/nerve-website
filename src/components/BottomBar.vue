<template>
  <div class="bottom cb">
    <div class="w1200">
      <div class="bottom-logo fl">
        <img class="bottom-logo" @click="toUrl('home')" src="./../assets/logo-w.svg">
        <p class="font14">Nerve Foundation</p>
        <p class="font14">Singapore</p>
      </div>
      <div class="bottom-right fr">
        <div class="menu fl">
          <el-menu :default-active="activeIndex" mode="horizontal" active-text-color="#79a7e4" @select="handleSelect">
            <el-menu-item index="home">{{$t('nav.home')}}</el-menu-item>
            <el-menu-item index="scene">{{$t('nav.scene')}}</el-menu-item>
            <!-- <el-menu-item index="wiring">线路图</el-menu-item>-->
            <el-menu-item index="library">{{$t('nav.library')}}</el-menu-item>
<!--            <el-menu-item index="team">{{$t('nav.team')}}</el-menu-item>-->
            <el-menu-item index="whiteBook">{{$t('nav.whiteBook')}}</el-menu-item>
          </el-menu>
        </div>
        <div class="community fr ">
          <ul>
            <li class="clicks fl">
              <svg id="icon-github" viewBox="0 0 50 50" @click="toUrl('https://github.com/NerveNetwork',1)">
                <path fill-rule="evenodd"
                      d="M25 0C11.2 0 0 11.467 0 25.597c0 11.262 7.2 20.886 17.1 24.265 1.2.205 1.7-.512 1.7-1.229v-4.3c-6.9 1.536-8.4-3.379-8.4-3.379-1.1-2.969-2.8-3.788-2.8-3.788-2.3-1.536.2-1.536.2-1.536 2.5.205 3.8 2.662 3.8 2.662 2.2 3.891 5.8 2.765 7.3 2.15.2-1.638.9-2.764 1.6-3.378C15 36.45 9.1 34.197 9.1 24.47c0-2.764 1-5.119 2.6-6.86-.3-.614-1.1-3.276.2-6.757 0 0 2.1-.717 6.9 2.662 2-.614 4.1-.82 6.3-.82 2.1 0 4.3.308 6.3.82 4.8-3.276 6.9-2.662 6.9-2.662 1.4 3.481.5 6.143.2 6.757 1.6 1.741 2.6 4.096 2.6 6.86 0 9.83-5.8 11.98-11.4 12.594.9.819 1.7 2.355 1.7 4.71v6.962c0 .717.4 1.433 1.7 1.228C42.8 46.381 50 36.86 50 25.597 50 11.467 38.8 0 25 0z"></path>
              </svg>
            </li>
            <li class="fl">
              <svg id="icon-telegram" viewBox="0 0 50 50" @click="toUrl('https://t.me/NerveNetwork',1)">
                <path d="M25 0c13.8 0 25 11.2 25 25S38.8 50 25 50 0 38.8 0 25 11.2 0 25 0zm11.6 15c.1-.5-.3-1-.6-.9-.1 0-.2.1-.3.1l-25.2 9.6c-.7.2-.7 1.3 0 1.5l5.8 2 3.5 7c0 .1.2.2.3.2 0 0 .1 0 .2-.1l3.3-2.8 5.4 4.1c.3.2.7.3 1 .3.7 0 1.4-.5 1.7-1.3L36.6 15zm-19 11.9l14-8.4-11.7 10.2.3 3.7-2.6-5.5z"></path>
              </svg>
            </li>
            <li class="clicks fl">
              <svg id="icon-facebook" viewBox="0 0 50 50"
                   @click="toUrl('https://www.facebook.com/groups/NerveNetwork',1)">
                <path d="M50.2,25.2C50.2,11.3,38.9,0,25,0S-0.2,11.3-0.2,25.2c0,12.6,9.2,23,21.2,24.8V32.4h-6.4v-7.3h6.4v-5.5 c0-6.3,3.8-9.8,9.5-9.8c2.8,0,5.6,0.5,5.6,0.5v6.2H33c-3.1,0-4.1,1.9-4.1,3.9v4.7h7l-1.1,7.3h-5.9V50C41,48.1,50.2,37.7,50.2,25.2z"></path>
              </svg>
            </li>
            <li class="fl">
              <svg id="icon-twitter" viewBox="0 0 50 50" @click="toUrl('https://twitter.com/nerve_network',1)">
                <path d="M50 25c0 13.8-11.2 25-25 25S0 38.8 0 25 11.2 0 25 0s25 11.2 25 25zM20.4 38.2c11.1 0 17.1-9.2 17.1-17.1v-.8c1.2-.9 2.2-1.9 3-3.1-1.1.5-2.2.8-3.5 1 1.2-.8 2.2-1.9 2.7-3.3-1.2.7-2.5 1.2-3.8 1.5-1.1-1.2-2.7-1.9-4.4-1.9-3.3 0-6 2.7-6 6 0 .5 0 .9.2 1.4-5-.2-9.4-2.6-12.4-6.3-.5.9-.8 1.9-.8 3 0 2.1 1.1 3.9 2.7 5-1 0-1.9-.3-2.7-.8v.1c0 2.9 2.1 5.4 4.8 5.9-.5.1-1 .2-1.6.2-.4 0-.8 0-1.1-.1.8 2.4 3 4.1 5.6 4.2-2.1 1.6-4.7 2.6-7.5 2.6-.5 0-1 0-1.4-.1 2.6 1.6 5.7 2.6 9.1 2.6z"></path>
              </svg>
            </li>
            <li class="clicks fl">
              <svg id="icon-medium" viewBox="0 0 50 50" @click="toUrl('https://medium.com/@NerveNetwork',1)">
                <path d="M25 0C11.2 0 0 11.2 0 25s11.2 25 25 25 25-11.2 25-25S38.8 0 25 0zm16.5 11.8l-2.7 2.6c-.2.2-.3.5-.3.8v18.9c0 .3.1.6.3.8l2.6 2.6v.6H28.3v-.6l2.7-2.6c.3-.3.3-.3.3-.8V18.7l-7.5 19.2h-1L14 18.7v12.8c-.1.5.1 1.1.5 1.5l3.5 4.3v.6H8v-.6l3.5-4.3c.4-.4.5-.9.5-1.5V16.7c0-.4-.1-.8-.4-1.1l-3.1-3.8v-.6h9.7l7.5 16.5 6.6-16.5h9.3v.6h-.1z"></path>
              </svg>
            </li>

          </ul>
        </div>
      </div>
    </div>
  </div>
</template>

<script>
  export default {
    name: "bottom-bar",
    data() {
      return {
        activeIndex: '1', //导航连接
      };
    },
    created() {
      let lang = navigator.language || navigator.userLanguage;//常规浏览器语言和IE浏览器
      if (sessionStorage.hasOwnProperty('lang')) {
        this.lang = sessionStorage.getItem('lang')
      } else {
        if (lang.substr(0, 2) === 'zh') {
          this.lang = 'cn'
        } else {
          this.lang = 'en'
        }
      }
      this.$i18n.locale = this.lang;
    },
    methods: {

      /**
       * @disc:导航连接
       * @params: key
       * @date: 2019-11-07 14:16
       * @author: Wave
       */
      handleSelect(key) {
        //console.log(key);
        if (key === 'scene' || key === 'team' || key === 'home') {
          this.toUrl(key)
        } else if (key === 'library') {
          window.open('https://github.com/NerveNetwork/nerve-docs')
        } else if (key === 'whiteBook') {
          const url = this.$i18n.locale === 'en' ?
            "http://nervefiles.oss-us-west-1.aliyuncs.com/wp/Nerve_WhitePaper_v1.00.pdf"
            : "http://nerve-cn.oss-cn-hangzhou.aliyuncs.com/wp/Nerve_WhitePaper_v1.00_cn.pdf"
          window.open(url)
        }
      },

      /**
       * 连接跳转
       * @param name , type 0:路由跳转 1：外网连接
       */
      toUrl(name, type = 0) {
        if (type === 0) {
          this.$router.push({
            name: name,
          })
        } else {
          window.open(name)
        }
      },
      openLink(link) {
        window.open(link)
      }
    }
  }
</script>

<style lang="less">
  .bottom {
    background-color: #1a56a4;
    width: 100%;
    height: 260px;
    .bottom-logo {
      width: 250px;
      .bottom-logo {
        width: 173px;
        height: 45px;
        margin: 50px 0;
      }
      p {
        color: #ffffff;
        line-height: 20px;
      }
    }
    .bottom-right {
      .menu {
        width: 480px;
        margin: 50px 0 0 0;
        .el-menu {
          background-color: transparent;
          .el-menu-item {
            color: #ffffff;
            &:hover {
              background-color: transparent;
            }
          }
          .is-active {
            background-color: #1a56a4 !important;
            border-bottom: 0;
          }
        }
      }
      .community {
        width: 310px;
        height: 50px;
        margin: 180px 0 0 0;
        ul {
          li {
            padding: 0 5px;
            font-size: 14px;
            &:first-child {
              /*padding: 0;*/
            }
            &:last-child {
              font-size: 14px;
              padding: 0 0 0 5px;
            }
            svg {
              cursor: pointer;
              width: 25px;
              fill: #a4c8f7;
            }
          }
        }
      }

    }
  }

</style>
