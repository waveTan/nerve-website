<template>
  <div class="scene">

    <div class="nerve">
      <div class="w1200">
        <h2 class="title">Nerve 连接区块链孤岛的桥</h2>
        <p class="info">
          Nerve提供了一套去中心化的数字资产服务网络。旨在打破区块链价值孤岛，建立跨链互通的资产交互网络，为Defi应用生态提供一切需要的底层支持。让数字资产持有者享受真正安全、自由、透明的Defi应用服务。</p>
      </div>
    </div>

    <div class="application">
      <div class="w1200">
        <h2 class="title tc">应用场景</h2>
        <p class="info tc">Nerve专为满足您的跨链需求而量身定制，为Defi应用生态提供一切需要的底层支持。</p>
      </div>
    </div>

    <div class="exchange">
      <div class="w1200">
        <div class="fl">
          <h2 class="title">交易所</h2>
          <p class="info">对比特币、以太坊、币安链等独立的公链，Nerve定义一套接口协议，可以方便的实现各种不同区块链的交互。</p>
        </div>
        <div class="fr">
          <img src="./../assets/img/header-bg.png">
        </div>
      </div>
    </div>

    <div class="payment">
      <div class="w1200">
        <div class="fl">
          <img src="./../assets/img/header-bg.png">
        </div>
        <div class="fr">
          <h2 class="title">快速支付</h2>
          <p class="info">对比特币、以太坊、币安链等独立的公链，Nerve定义一套接口协议，可以方便的实现各种不同区块链的交互。</p>
        </div>
      </div>
    </div>

    <div class="Settlement">
      <div class="w1200">
        <div class="fl">
          <h2 class="title">跨币种清算/结算</h2>
          <p class="info">Nerve的通用跨链协议，支持不同币种间进行跨币种清算/结算</p>
        </div>
        <div class="fr">
          <img src="./../assets/img/header-bg.png">
        </div>
      </div>
    </div>

    <div class="staking">
      <div class="w1200">
        <div class="fl">
          <img src="./../assets/img/header-bg.png">
        </div>
        <div class="fr">
          <h2 class="title">多资产Staking</h2>
          <p class="info">可用多种不同资产，跨资产参与Nerve共识节点的建设和委托，在保障节点正常运营的同时，获得共识奖励。</p>
        </div>
      </div>
    </div>

    <div class="more tc">
      <h2 class="title">更多场景</h2>
      <p class="info">开放的基因即将涌现更多的可能性</p>
    </div>

  </div>
</template>

<script>
  export default {
    name: 'home',
  }
</script>
<style lang="less">
  .scene {
    .nerve {
      height: 650px;
      padding-top: 200px;
      .info {
        width: 50%;
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
