<template>
  <div class="partner">
    <div class="nerve">
      <div class="w1200">
        <div class="fl">
          <h2 class="title">{{$t('partners.partners0')}}</h2>
          <p class="info">{{$t('partners.partners1')}}</p>
        </div>
        <div class="fr">
          <img src="./../assets/img/partner_bg.svg">
        </div>
      </div>
    </div>
    <div class="partner_list">
      <div class="w1200">
        <h2 class="title tc">{{$t('partners.partners2')}}</h2>
        <ul>
          <li class="fl click" @click="toUrl('https://www.nuls.io/')"><img src="@/assets/img/Nerve_03.png"></li>
          <li class="fl click" @click="toUrl('http://nabox.io/')"><img src="@/assets/img/Nerve_05.png"></li>
          <li class="fl click" @click="toUrl('https://bscscan.com/')"><img src="@/assets/img/bsc.png"></li>
          <li class="fl click" @click="toUrl('https://okex.com/okchain')"><img src="@/assets/img/Nerve_06.png"></li>
          <li class="fl click" @click="toUrl('https://www.slowmist.com/')"><img src="@/assets/img/manwu.png"></li>
          <li class="fl click" @click="toUrl('https://app.uniswap.org/#/swap')"><img src="@/assets/img/uniswap.png">
          </li>
          <li class="fl click" @click="toUrl('https://www.chainsguard.com/index.html#home')"><img
                  src="@/assets/img/lianan.png"></li>
          <li class="fl click" @click="toUrl('https://pancakeswap.finance/')"><img src="@/assets/img/pancake.png"></li>
        </ul>
      </div>
    </div>
    <div class="cb"></div>
    <div class="partner_list" style="min-height: 600px">
      <div class="w1200">
        <h2 class="title tc">{{$t('partners.partners3')}}</h2>
        <ul>
          <li class="fl click" @click="toUrl('https://www.bitz.cm/')"><img src="@/assets/img/Nerve_09.png"></li>
          <li class="fl click" @click="toUrl('https://www.tokenbetter.com/vc/')"><img src="@/assets/img/Nerve_10.png">
          </li>
          <li class="fl click" @click="toUrl('http://www.xstarpool.com/')"><img src="@/assets/img/Nerve_11.png"></li>
          <li class="fl click" @click="toUrl('http://www.imgfund.com/')"><img src="@/assets/img/Nerve_12.png"></li>
          <li class="fl click"><img src="@/assets/img/Nerve_13.png"></li>
          <!--<li class="fl click" v-for="item of mediaData" :key="item.key" @click="toUrl(item.url)">
            <img :src="item.imgUrl">
          </li>-->
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
          {key: 0, url: 'https://www.nuls.io/', imgUrl: "NULS.jpg"},
          {key: 1, url: 'https://usdi.co/', imgUrl: "usdi.png"},
          {key: 2, url: 'http://nabox.io/', imgUrl: " nabox.png"},
          {key: 3, url: 'https://okex.com/okchain', imgUrl: " okchain.png"}
        ], //战略合作

        mediaData: [
          {key: 0, url: 'http://www.imgfund.com/', imgUrl: "imagine.png"},
          {key: 1, url: 'https://www.tokenbetter.com/vc/', imgUrl: "TB.png"},
          {key: 2, url: 'https://www.bitz.cm/', imgUrl: "bitz.PNG"},
          {key: 3, url: 'www.xstarpool.com', imgUrl: "future.png"},
          {key: 4, url: '', imgUrl: "index.png"}
        ], //媒体伙伴
      }
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
      height: 720px;
      padding-top: 150px;
      .fl {
        width: 600px;
      }
      .fr {
        width: 600px;
        text-align: right;
        img {
          width: 450px;
          margin: 0 0 0 100px;
        }
      }

    }
    .partner_list {
      min-height: 400px;
      ul {
        margin: 20px 0 20px 0;
        li {
          width: 25%;
          height: 200px;
          text-align: center;
          margin: 0;
          &:first-child {
            margin-left: 0;
          }
          &:last-child {
            margin-right: 0;
          }
          img {
            width: 380px;
            height: 190px;
          }
        }
      }
    }
  }
</style>
