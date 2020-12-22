<template>
  <div class="header">
    <div class="w1200">
      <div class="logo fl">
        <div class="click img" @click="toUrl('home')"></div>
      </div>
      <div class="menu fl">
        <el-menu :default-active="activeIndex" mode="horizontal" active-text-color="#79a7e4" @select="handleSelect">
          <el-menu-item index="scene">{{$t('nav.scene')}}</el-menu-item>
          <el-menu-item index="partners">{{$t('partners.partners0')}}</el-menu-item>
          <el-menu-item index="NerveDex">NerveDEX</el-menu-item>
          <!-- <el-menu-item index="wiring">线路图</el-menu-item>-->
          <!--<el-menu-item index="wallet">{{$t('nav.wallet')}}</el-menu-item>-->
          <el-submenu index="wallet" :popper-append-to-body="false">
            <template slot="title">{{$t('nav.wallet')}}</template>
            <!--<el-menu-item index="desktop">
              <span @click="handleSelect('desktop')">{{$t('nav.desktop')}}</span>
            </el-menu-item>-->
            <el-menu-item index="web-wallet">
              <span @click="handleSelect('webWallet')">{{$t('nav.webWallet')}}</span>
            </el-menu-item>
            <el-menu-item index="light-wallet">
              <span @click="handleSelect('desktop')">{{$t('nav.desktop')}}</span>
            </el-menu-item>
          </el-submenu>


          <el-menu-item index="browser">{{$t('nav.browser')}}</el-menu-item>
          <el-submenu index="2" :popper-append-to-body="false">
            <template slot="title">{{$t('nav.about')}}</template>
            <!--<el-menu-item index="desktop">
              <span @click="handleSelect('desktop')">{{$t('nav.desktop')}}</span>
            </el-menu-item>-->
            <el-menu-item index="library">
              <span @click="handleSelect('library')">{{$t('nav.library')}}</span>
            </el-menu-item>
            <el-menu-item index="whiteBook">
              <span @click="handleSelect('whiteBook')">{{$t('nav.whiteBook')}}</span>
            </el-menu-item>
          </el-submenu>
        </el-menu>
        <div class="language fr font14 click" @click="selectLanguage">{{lang === 'en' ? '简体中文':'English' }}</div>
      </div>
    </div>
  </div>
</template>

<script>
  export default {
    data() {
      return {
        activeIndex: '1', //导航连接
        lang: 'en', //语言
      };
    },
    created() {
      sessionStorage.setItem('lang', 'en');
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
        if (key === 'scene' || key === 'team' || key === 'partners') {
          this.toUrl(key)
        } else if (key === 'NerveDex') {
          window.open('https://nervedex.com/')
        } else if (key === 'library') {
          const url = this.$i18n.locale === 'en' ? "http://docs.nerve.network/" : "http://docs.nerve.network/zh/";
          window.open(url)
        } else if (key === 'whiteBook') {
          const url = this.$i18n.locale === 'en' ?
            "http://nervefiles.oss-us-west-1.aliyuncs.com/wp/Nerve_Whitepaper_EN.pdf"
            : "http://nerve-cn.oss-cn-hangzhou.aliyuncs.com/wp/Nerve_Whitepaper_ZH.pdf";
          window.open(url)
        } else if (key === 'webWallet') {
          window.open('https://wallet.nerve.network/')
        } else if (key === 'browser') {
          window.open('https://scan.nerve.network/')
        } else if (key === 'desktop') {
          window.open('https://github.com/NerveNetwork/nerve/releases')
        }
      },

      /**
       * 语言切换
       */
      selectLanguage() {
        if (this.lang === 'en') {
          this.lang = 'cn'
        } else {
          this.lang = 'en'
        }
        sessionStorage.setItem('lang', this.lang);
        this.$i18n.locale = this.lang;
      },

      /**
       * url 连接
       * @param name
       * @param type 0:路由跳转 1:连接跳转
       */
      toUrl(name, type = 0) {
        this.$router.push({
          name: name,
        })
      }
    }
  }
</script>

<style lang="less">
  .header {
    height: 100px;
    @media screen and (max-width: 1750px) {
      background-color: #1a56a4;
    }

    .logo {
      width: 15%;
      margin: 20px 0 0 0;
      .img {
        width: 200px;
        height: 73px;
        background: url("./../assets/logo.svg") no-repeat;
        @media screen and (max-width: 1770px) {
          background: url("./../assets/logo-w.svg") no-repeat;
        }
      }
    }
    .menu {
      width: 65%;
      margin-left: 20%;
      .el-menu {
        background-color: transparent;
        margin: 40px 0 0 0;
        height: 30px;
        width: 80%;
        .el-menu-item, .el-submenu__title {
          color: #ffffff;
          line-height: 20px;
          height: 20px;
          &:hover {
            background-color: transparent;
            color: #ffffee;
          }
        }
        .is-active {
          background-color: #1a56a4 !important;
          border-bottom: 0;
        }
        .el-submenu {
          .el-menu {
            margin-top: 0;
          }
          .el-submenu__title {
            color: #ffffee;
            border-bottom: none !important;
          }
          .el-menu-item {
            background-color: #1a56a4;
            line-height: 36px;
            height: 36px;
            color: #ffffee;
            min-width: 150px;
            &:hover {
              color: #79a7e4;
            }
          }
        }
      }
      .language {
        margin: -25px 0 0 0;
        height: 20px;
        color: #ffffff;
      }
    }

  }
</style>
