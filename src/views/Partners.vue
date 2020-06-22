<template>
  <div class="partner">
    <div class="nerve">
      <div class="w1200">
        <div class="fl">
          <h2 class="title">合作伙伴</h2>
          <p class="info">Nerve为众多合作伙伴提供了稳定高效的去中心化网络服务，同时各个合作伙伴也伴随着Nerve的成长</p>
        </div>
        <div class="fr">
          <img src="./../assets/img/bg1.png">
        </div>
      </div>
    </div>
    <div class="partner_list">
      <div class="w1200">
        <h2 class="title tc">战略合作</h2>
        <ul>
          <li class="fl click" v-for="item of strategicData" :key="item.key" @click="toUrl(item.url)">
            <img :src="item.imgUrl">
          </li>
        </ul>
      </div>
    </div>
    <div class="cb"></div>
    <div class="partner_list">
      <div class="w1200">
        <h2 class="title tc">媒体伙伴</h2>
        <ul>
          <li class="fl click" v-for="item of mediaData" :key="item.key" @click="toUrl(item.url)">
            <img :src="item.imgUrl">
          </li>
        </ul>
      </div>
    </div>
    <div class="cb"></div>
  </div>
</template>

<script>
  export default {
    data() {
      return {
        strategicData: [
          {key: 0, url: 'https://www.baidu.com', imgUrl: "https://nulscan.io/dist/img/logo.ef0bcec3.svg"},
          {key: 1, url: 'https://www.baidu.com', imgUrl: "https://nulscan.io/dist/img/logo.ef0bcec3.svg"},
          {key: 2, url: 'https://www.baidu.com', imgUrl: "https://nulscan.io/dist/img/logo.ef0bcec3.svg"},
          {key: 3, url: 'https://www.baidu.com', imgUrl: "https://nulscan.io/dist/img/logo.ef0bcec3.svg"},
        ], //战略合作

        mediaData: [
          {key: 0, url: 'https://www.baidu.com', imgUrl: "https://nulscan.io/dist/img/logo.ef0bcec3.svg"},
          {key: 1, url: 'https://www.baidu.com', imgUrl: "https://nulscan.io/dist/img/logo.ef0bcec3.svg"},
          {key: 2, url: 'https://www.baidu.com', imgUrl: "https://nulscan.io/dist/img/logo.ef0bcec3.svg"},
          {key: 3, url: 'https://www.baidu.com', imgUrl: "https://nulscan.io/dist/img/logo.ef0bcec3.svg"},
        ], //媒体伙伴

      };
    },
    created() {

    },
    methods: {

      /**
       * url 连接
       * @param name
       */
      toUrl(name) {
        window.open(name)
      }
    }
  }
</script>
<style lang="less">
  .partner {
    .nerve {
      height: 500px;
      padding-top: 100px;
      .fl {
        width: 600px;
      }
      .fr {
        width: 600px;
        text-align: right;
        img {
          width: 582px;
          margin-top: -100px;
        }
      }

    }
    .partner_list {
      height: 400px;
      ul {
        margin: 40px 0 0 0;
        li {
          width: 25%;
          height: 70px;
          text-align: center;
          &:first-child {
            margin-left: 0;
          }
          &:last-child {
            margin-right: 0;
          }
          img {
            width: 160px;
            height: 40px;
          }
        }
      }
    }
  }
</style>
