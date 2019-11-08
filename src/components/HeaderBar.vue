<template>
  <div class="header">
    <div class="w1200">
      <div class="logo fl">
        <img class="click" @click="toUrl('home')" src="./../assets/logo.svg">
      </div>
      <div class="menu fl">
        <el-menu :default-active="activeIndex" mode="horizontal" active-text-color="#79a7e4" @select="handleSelect">
          <el-menu-item index="scene">{{$t('nav.scene')}}</el-menu-item>
         <!-- <el-menu-item index="wiring">线路图</el-menu-item>-->
          <el-menu-item index="library">{{$t('nav.library')}}</el-menu-item>
          <el-menu-item index="team">{{$t('nav.team')}}</el-menu-item>
          <el-menu-item index="whiteBook">{{$t('nav.whiteBook')}}</el-menu-item>
          <div class="language fr font14 click" @click="selectLanguage">{{lang === 'en' ? '简体中文':'English' }}</div>
        </el-menu>
      </div>
    </div>
  </div>
</template>

<script>
  export default {
    data() {
      return {
        activeIndex: '1', //导航连接
        lang: 'cn', //语言
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
        if (key === 'scene') {
          this.toUrl(key)
        } else if (key === 'team') {
          this.toUrl(key)
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
    .logo {
      width: 201px;
      margin: 15px 0 0 0;
      img {
        width: 100%;
        height: 73px;
      }
    }
    .menu {
      width: 799px;
      margin-left: 520px;
      .el-menu {
        background-color: transparent;
        margin: 40px 0 0 0;
        height: 30px;
        .el-menu-item {
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
      }
    }
    .language {
      margin: 5px 0 0 0;
      height: 20px;
      color: #ffffff;
    }
  }
</style>
