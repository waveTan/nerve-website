<template>
  <div class="team">
    <div class="team-list w1200">
      <h3 class="tc" style="color: #ffffff" >发起人</h3>
      <ul class="tc">
        <li>
          <h6><img src="./../assets/team/Berzeck.png"></h6>
          <h5>Mario Blacutt Bolivia</h5>
          <p>发起人</p>
        </li>
      </ul>
    </div>
    <div class="cb"></div>
    <div class="team-list w1200">
      <h3 class="tc">团队</h3>
      <ul>
        <li class="fl">
          <h6><img src="./../assets/team/LIN-2.jpg"></h6>
          <h5>Lin Yang</h5>
          <p>架构师-中国</p>
        </li>
        <li class="fl">
          <h6><img src="./../assets/team/Niels.png"></h6>
          <h5>Niels Wang</h5>
          <p>架构师-中国</p>
        </li>
        <li class="fl">
          <h6><img src="./../assets/team/Moshe.png"></h6>
          <h5>Moshe</h5>
          <p>全栈工程师-法国</p>
        </li>
        <li class="fl">
          <h6><img src="./../assets/team/Angel.png"></h6>
          <h5>Angel</h5>
          <p>全栈工程师-西班牙</p>
        </li>
        <li class="fl">
          <h6><img src="./../assets/team/Claudio.png"></h6>
          <h5>Claudio</h5>
          <p>UI/UX设计师-比利时</p>
        </li>
        <li class="fl">
          <h6><img src="./../assets/team/Naveen.png"></h6>
          <h5>Naveen</h5>
          <p>Java工程师-新加坡</p>
        </li>
        <li class="fl">
          <h6><img src="./../assets/team/Edward.png"></h6>
          <h5>Edward</h5>
          <p>架构师-中国</p>
        </li>
        <li class="fl">
          <h6><img src="./../assets/team/nalex.jpeg"></h6>
          <h5>Nalex</h5>
          <p>动画设计师 - 澳大利亚</p>
        </li>
        <li class="fl">
          <h6><img src="./../assets/team/Pen-Luo.jpg"></h6>
          <h5>Pen</h5>
          <p>产品经理</p>
        </li>
        <li class="fl">
          <h6><img src="./../assets/team/long-1.jpeg"></h6>
          <h5>Long</h5>
          <p>Jave工程师-中国</p>
        </li>
        <li class="fl">
          <h6><img src="./../assets/team/peak.jpeg"></h6>
          <h5>Peak</h5>
          <p>Jave工程师-中国</p>
        </li>
        <li class="fl">
          <h6><img src="./../assets/team/Tudor.jpeg"></h6>
          <h5>Tudor</h5>
          <p>全栈工程师 - 澳大利亚</p>
        </li>
        <li class="fl">
          <h6><img src="./../assets/team/kathy.jpeg"></h6>
          <h5>Kathy</h5>
          <p>架构师-美国</p>
        </li>
        <li class="fl">
          <h6><img src="./../assets/team/Cody-Lan.jpg"></h6>
          <h5>Cody Lan</h5>
          <p>架构师-中国</p>
        </li>
        <li class="fl">
          <h6><img src="./../assets/team/Wave-Tan.jpg"></h6>
          <h5>Wave Tan</h5>
          <p>前端工程师-中国</p>
        </li>
        <li class="fl">
          <h6><img src="./../assets/team/WechatIMG212.jpeg"></h6>
          <h5>Lijun Zhou</h5>
          <p>架构师-中国</p>
        </li>
        <li class="fl">
          <h6><img src="./../assets/team/Charlie-Li.jpg"></h6>
          <h5>Charlie Li</h5>
          <p>Java工程师-中国</p>
        </li>
        <li class="fl">
          <h6><img src="./../assets/team/Pierre-Luo.jpg"></h6>
          <h5>Pierre Luo</h5>
          <p>架构师-中国</p>
        </li>
        <li class="fl">
          <h6><img src="./../assets/team/ViVi-zhou.jpg"></h6>
          <h5>ViVi Zhou</h5>
          <p>架构师-中国</p>
        </li>
        <li class="fl">
          <h6><img src="./../assets/team/Albert-Yi.jpg"></h6>
          <h5>Albert Yi</h5>
          <p>测试工程师-中国</p>
        </li>
        <li class="fl">
          <h6><img src="./../assets/team/Angang-Tang.jpg"></h6>
          <h5>Angang Tang</h5>
          <p>Java工程师-中国</p>
        </li>
      </ul>
    </div>
  </div>
</template>

<script>
  export default {
    name: 'team',
  }
</script>
<style lang="less">
  .team {
    height: 800px;
    .team-list {
      h3 {
        width: 300px;
        margin: 50px auto 100px;
        font-size: 4rem;
        font-weight: 700;
        padding-bottom: 1.4rem;
        border-bottom: 0.4rem solid #1a56a4;
      }
      ul {
        li {
          margin: 0 4rem 5rem 0;
          &:nth-child(4n) {
            margin-right: 0;
          }
          h6 {
            margin-bottom: 2rem;
            margin-left: auto;
            margin-right: auto;
            text-align: center;
            img {
              max-width: 20rem;
              border-radius: 1rem;
              box-shadow: 0.2rem 0.4rem 1.2rem 0.2rem;
            }
          }
          h5 {
            margin-bottom: 1.5rem;
            font-size: 2rem;
            font-weight: 700;
            line-height: 1.14286;
            text-align: center;
          }
          p {
            margin-left: auto;
            margin-right: auto;
            max-width: 24rem;
            color: #1a56a4;
            font-size: 1.5rem;
            font-weight: 500;
            line-height: 1.33333;
            text-align: center;
          }
        }
      }
    }
  }
</style>
