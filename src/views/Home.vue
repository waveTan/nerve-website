<template>
  <div class="home">

    <div class="nerve">
      <div class="w1200">
        <h2 class="title">{{$t('home.home0')}}</h2>
        <p class="info">{{$t('home.home1')}}</p>
      </div>
    </div>

    <div class="trait">
      <div class="w1200">
        <h2 class="title tc">{{$t('home.home2')}}</h2>
        <ul>
          <li class="fl">
            <img src="./../assets/img/trait1.png">
            <h3 class="font20">{{$t('home.home3')}}</h3>
            <p class="font14">{{$t('home.home4')}}</p>
          </li>
          <li class="fl">
            <img src="./../assets/img/trait2.png">
            <h3>{{$t('home.home5')}}</h3>
            <p>{{$t('home.home6')}}</p>
          </li>
          <li class="fl">
            <img src="./../assets/img/trait3.png">
            <h3>{{$t('home.home7')}}</h3>
            <p>{{$t('home.home8')}}</p>
          </li>
        </ul>
      </div>
    </div>

    <div class="what-Nerve">
      <div class="w1200">
        <h2 class="title tc">{{$t('home.home9')}}</h2>
        <p class="info">{{$t('home.home10')}}</p>
        <ul>
          <li class="fl">
            <img src="./../assets/img/whatNerve1.png">
            <h3>{{$t('home.home11')}}</h3>
            <p>{{$t('home.home12')}}</p>
          </li>
          <li class="fl">
            <img src="./../assets/img/whatNerve2.png">
            <h3>{{$t('home.home13')}}</h3>
            <p>{{$t('home.home14')}}</p>
          </li>
          <li class="fl">
            <img src="./../assets/img/whatNerve3.png">
            <h3>{{$t('home.home15')}}</h3>
            <p>{{$t('home.home16')}}</p>
          </li>
          <li class="fl">
            <img src="./../assets/img/whatNerve4.png">
            <h3>{{$t('home.home17')}}</h3>
            <p>{{$t('home.home18')}}</p>
          </li>
        </ul>
      </div>
    </div>

    <div class="cross-link">
      <div class="w1200">
        <div class="fl">
          <h2 class="title">{{$t('home.home19')}}</h2>
          <p class="info">{{$t('home.home20')}}</p>
        </div>
        <div class="fr">
          <img src="./../assets/img/crossLink1.png">
        </div>
      </div>
    </div>

    <div class="consensus">
      <div class="w1200">
        <div class="fl">
          <img src="./../assets/img/consensus1.png">
        </div>
        <div class="fr">
          <h2 class="title">{{$t('home.home21')}}</h2>
          <p class="info">{{$t('home.home22')}}</p>
        </div>
      </div>
    </div>

    <div class="feed">
      <div class="w1200">
        <div class="fl">
          <h2 class="title">{{$t('home.home23')}}</h2>
          <p class="info">{{$t('home.home24')}}</p>
        </div>
        <div class="fr">
          <img src="./../assets/img/feed1.png">
        </div>
      </div>
    </div>

    <div class="line">
      <h2 class="title tc">{{$t('home.home25')}}</h2>
      <div class="line-top w1200">
        <div class="fl one">
          <img class="fl" src="./../assets/img/fine1.png">
          <div class="fl">
            <h3>{{$t('home.home26')}}</h3>
            <p>{{$t('home.home27')}}</p>
          </div>
        </div>
        <div class="fl two">
          <img class="fl" src="./../assets/img/fine2.png">
          <div class="fl">
            <h3>{{$t('home.home28')}}</h3>
            <p>{{$t('home.home29')}}</p>
          </div>
        </div>
      </div>
      <div class="line-middle cb">
        <ul class="w1200">
          <li class="fl"><font></font><span>2020-Q1</span></li>
          <li class="fl"><font></font><span>2020 Q2&Q3</span></li>
          <li class="fl"><font></font><span>2020 Q4</span></li>
          <li class="fl"><font></font><span>2021-2023</span></li>
        </ul>
      </div>
      <div class="line-bottom w1200">
        <div class="fl one">
          <img class="fl" src="./../assets/img/fine3.png">
          <div class="fl">
            <h3>{{$t('home.home30')}}</h3>
            <p>{{$t('home.home31')}}</p>
          </div>
        </div>
        <div class="fl two">
          <img class="fl" src="./../assets/img/fine4.png">
          <div class="fl infos">
            <h3>{{$t('home.home32')}}</h3>
            <p>{{$t('home.home33')}}</p>
          </div>
        </div>
      </div>
    </div>

    <div class="partner" v-show="false">
      <div class="w1200">
        <h2 class="title tc">{{$t('home.home34')}}</h2>
        <ul>
          <li class="fl">
            <img src="./../assets/img/partner1.png">
          </li>
          <li class="fl">
            <img src="./../assets/img/partner2.png">
          </li>
          <li class="fl">
            <img src="./../assets/img/partner1.png">
          </li>
          <li class="fl">
            <img src="./../assets/img/partner2.png">
          </li>
          <li class="fl">
            <img src="./../assets/img/partner1.png">
          </li>
          <li class="fl">
            <img src="./../assets/img/partner2.png">
          </li>
          <li class="fl">
            <img src="./../assets/img/partner1.png">
          </li>
          <li class="fl">
            <img src="./../assets/img/partner2.png">
          </li>
        </ul>
      </div>
    </div>
    <div class="cb"></div>

  </div>
</template>

<script>
  export default {
    name: 'home',
    data() {
      return {};
    },
    components: {},
    watch: {},
    created() {
    },
    mounted() {
    },
    methods: {}
  }
</script>
<style lang="less">
  .home {
    .nerve {
      height: 750px;
      padding-top: 300px;
    }
    .trait {
      height: 800px;
      margin: 120px 0 0 0;
      .title {
        margin: 0 0 120px 0;
      }
      ul {
        li {
          width: 300px;
          height: 400px;
          //border-bottom: 3px solid linear-gradient(to right, #18e9d9, #5f7aea);
          border-bottom: 10px solid #18e9d9;
          margin: 20px 70px 0;
          border-radius: 10px;
          background-color: #ffffff;
          text-align: center;
          &:first-child {
            margin-left: 0;
          }
          &:last-child {
            margin-right: 0;
          }
          @media screen and (min-width: 1520px) {
            margin: 20px 150px 0;
          }
          img {
            margin: 50px 80px;
            width: 155px;
            height: 155px;
            border-radius: 100px;
          }
          p {
            margin: 10px 0 0 0;
          }
        }
      }
    }
    .what-Nerve {
      height: 680px;
      .info {
        margin: 50px 0 150px 0;
        line-height: 30px;
      }
      ul {
        li {
          width: 270px;
          text-align: center;
          margin: 20px 18px 0 18px;
          &:first-child {
            margin-left: 0;
          }
          &:last-child {
            margin-right: 0;
          }
          @media screen and (min-width: 1520px) {
            margin: 20px 70px 0;
          }
          h3 {
            font-size: 22px;
            font-weight: bold;
            margin: 30px 0;
            height: 60px;
          }
          p {
            font-size: 18px;
            line-height: 26px;
            text-align: left;
          }
        }
      }
    }
    .cross-link {
      height: 650px;
      padding-top: 300px;
      .fl {
        width: 50%;
      }
      .fr {
        width: 50%;
        text-align: center;
      }
    }
    .consensus {
      height: 600px;
      padding-top: 200px;
      .fl {
        width: 50%;
        text-align: center;
      }
      .fr {
        width: 50%;

      }
    }
    .feed {
      height: 700px;
      padding-top: 200px;
      .fl {
        width: 50%;
      }
      .fr {
        width: 50%;
        text-align: center;
      }
    }
    .line {
      height: 860px;
      margin: 0 0 0 0;
      .line-top {
        height: 100px;
        margin: 50px auto 0;
        .fl {
          img {
            width: 100px;
            display: block;
          }
          h3 {
            font-size: 20px;
            color: #17202e;
            margin: 10px 0 0 10px;
          }
          p {
            font-size: 14px;
            width: 450px;
            margin: 0 0 0 10px;
          }
        }
        .one {
          width: 600px;
          margin-left: -40px;
        }
        .two {
          margin: 0 0 0 20px;
          @media screen and (min-width: 1520px) {
            margin: 0 0 0 170px;
          }
        }
      }
      .line-middle {
        height: 20px;
        border-top: 1px solid #1a56a4;
        margin: 20px 0 0 0;
        ul {
          li {
            width: 300px;
            @media screen and (min-width: 1520px) {
              width: 380px;
            }
            font {
              width: 20px;
              height: 20px;
              background-color: #39b4e1;
              display: block;
              border-radius: 10px;
              margin: -10px 0 0 0;
            }
          }
        }
      }
      .line-bottom {
        height: 200px;
        position: absolute;
        .fl {
          img {
            width: 100px;
          }
          h3 {
            font-size: 20px;
            color: #17202e;
            margin: 10px 0 0 10px;
          }
          p {
            font-size: 14px;
            width: 450px;
            margin: 0 0 0 10px;
          }
        }
        .one {
          margin: 40px 0 0 220px;
          z-index: 33;
          @media screen and (min-width: 1520px) {
            margin: 40px 0 0 460px;
          }
        }
        .two {
          width: 400px;
          margin: 40px 0 0 50px;
          position: absolute;
          z-index: 33;
          img {
            width: 110px;
            float: left;
          }
          .infos {
            width: 250px;
            h3, p {
              width: 400px;
              @media screen and (min-width: 1520px) {
                width: 525px;
              }
            }
          }
          @media screen and (min-width: 1520px) {
            width: 560px;
            margin: 40px 0 0 200px;
            img {
              width: 110px;
              float: left;
            }

            .infos {
              width: 450px;
            }
          }
        }
      }
    }
    .partner {
      height: 510px;
      ul {
        li {
          width: 25%;
          text-align: center;
          margin: 20px 0 20px 0;
          img {
            width: 160px;
            height: 70px;
          }
        }
      }
    }

  }
</style>
