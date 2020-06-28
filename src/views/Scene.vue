<template>
  <div class="scene">

    <div class="nerve">
      <div class="w1200">
        <div class="fl">
          <h2 class="title">{{$t('scene.scene0')}}</h2>
          <p class="info">{{$t('scene.scene1')}}</p>
        </div>
        <div class="fr">
          <img src="./../assets/img/bg1.png">
        </div>
      </div>
    </div>

    <div class="application">
      <div class="w1200">
        <h2 class="title tc">{{$t('scene.scene2')}}</h2>
        <p class="info tc">{{$t('scene.scene3')}}</p>
      </div>
    </div>

    <div class="exchange">
      <div class="w1200">
        <div class="fl">
          <h2 class="title">{{$t('scene.scene4')}}</h2>
          <p class="info">{{$t('scene.scene5')}}</p>
        </div>
        <div class="fr">
          <img src="./../assets/img/bg2.png">
        </div>
      </div>
    </div>

    <div class="payment">
      <div class="w1200">
        <div class="fl">
          <img src="./../assets/img/bg3.png">
        </div>
        <div class="fr">
          <h2 class="title">{{$t('scene.scene6')}}</h2>
          <p class="info">{{$t('scene.scene7')}}</p>
        </div>
      </div>
    </div>

    <div class="Settlement">
      <div class="w1200">
        <div class="fl">
          <h2 class="title">{{$t('scene.scene8')}}</h2>
          <p class="info">{{$t('scene.scene9')}}</p>
        </div>
        <div class="fr">
          <img src="./../assets/img/bg4.png">
        </div>
      </div>
    </div>

    <div class="staking">
      <div class="w1200">
        <div class="fl">
          <img src="./../assets/img/bg5.png">
        </div>
        <div class="fr">
          <h2 class="title">{{$t('scene.scene10')}}</h2>
          <p class="info">{{$t('scene.scene11')}}</p>
        </div>
      </div>
    </div>

    <div class="more tc">
      <h2 class="title">{{$t('scene.scene12')}}</h2>
      <p class="info">{{$t('scene.scene13')}}</p>
    </div>
  </div>
</template>

<script>
  export default {
    name: 'scene',
  }
</script>
<style lang="less">
  .scene {
    .nerve {
      height: 800px;
      padding-top: 150px;
      .fl {
        width: 700px;
      }
      .fr {
        width: 500px;
        text-align: right;
        img {
          width: 500px;
          margin-top:10px;
        }
      }

    }
    .application {
      height: 300px;
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
    .exchange {
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
    .payment {
      height: 700px;
      padding-top: 200px;
      .fl {
        width: 50%;
        text-align: center;
      }
      .fr {
        width: 50%;

      }
    }
    .Settlement {
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
    .staking {
      height: 700px;
      padding-top: 200px;
      .fl {
        width: 50%;
        text-align: center;
      }
      .fr {
        width: 50%;

      }
    }
    .more {
      height: 200px;
    }
  }
</style>
