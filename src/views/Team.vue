<template>
  <div class="team">
    <div class="team-list w1200">
      <h3 class="tc fast">{{$t('team.team0')}}</h3>
      <ul class="tc">
        <li style="margin: 0">
          <h6><img src="./../assets/team/Berzeck.png"></h6>
          <h5>Berzeck</h5>
          <p>{{$t('team.team0')}}</p>
        </li>
      </ul>
    </div>
    <div class="cb"></div>
    <div class="team-list w1200">
      <h3 class="tc">{{$t('team.team1')}}</h3>
      <ul>
        <li class="fl">
          <h6><img src="./../assets/team/LIN-2.jpg"></h6>
          <h5>Lin Yang</h5>
          <p>{{$t('team.team2')}}-{{$t('team.team3')}}</p>
        </li>
        <li class="fl">
          <h6><img src="./../assets/team/Niels.png"></h6>
          <h5>Niels Wang</h5>
          <p>{{$t('team.team2')}}-{{$t('team.team3')}}</p>
        </li>
        <li class="fl">
          <h6><img src="./../assets/team/Moshe.png"></h6>
          <h5>Moshe</h5>
          <p>{{$t('team.team4')}}-{{$t('team.team5')}}</p>
        </li>
        <li class="fl">
          <h6><img src="./../assets/team/Angel.png"></h6>
          <h5>Angel</h5>
          <p>{{$t('team.team4')}}-{{$t('team.team6')}}</p>
        </li>
        <li class="fl">
          <h6><img src="./../assets/team/Claudio.png"></h6>
          <h5>Claudio</h5>
          <p>{{$t('team.team7')}}-{{$t('team.team8')}}</p>
        </li>
        <li class="fl">
          <h6><img src="./../assets/team/Naveen.png"></h6>
          <h5>Naveen</h5>
          <p>{{$t('team.team9')}}-{{$t('team.team10')}}</p>
        </li>
        <li class="fl">
          <h6><img src="./../assets/team/Edward.png"></h6>
          <h5>Edward</h5>
          <p>{{$t('team.team2')}}-{{$t('team.team3')}}</p>
        </li>
        <li class="fl">
          <h6><img src="./../assets/team/nalex.jpeg"></h6>
          <h5>Nalex</h5>
          <p>{{$t('team.team11')}} - {{$t('team.team12')}}</p>
        </li>
        <li class="fl">
          <h6><img src="./../assets/team/Pen-Luo.jpg"></h6>
          <h5>Pen</h5>
          <p>{{$t('team.team13')}}-{{$t('team.team3')}}</p>
        </li>
        <li class="fl">
          <h6><img src="./../assets/team/long-1.jpeg"></h6>
          <h5>Long</h5>
          <p>{{$t('team.team9')}}-{{$t('team.team3')}}</p>
        </li>
        <li class="fl">
          <h6><img src="./../assets/team/peak.jpeg"></h6>
          <h5>Peak</h5>
          <p>{{$t('team.team9')}}-{{$t('team.team3')}}</p>
        </li>
        <li class="fl">
          <h6><img src="./../assets/team/Tudor.jpeg"></h6>
          <h5>Tudor</h5>
          <p>{{$t('team.team4')}}-{{$t('team.team12')}}</p>
        </li>
        <li class="fl">
          <h6><img src="./../assets/team/kathy.jpeg"></h6>
          <h5>Kathy</h5>
          <p>{{$t('team.team2')}}-{{$t('team.team15')}}</p>
        </li>
        <li class="fl">
          <h6><img src="./../assets/team/Cody-Lan.jpg"></h6>
          <h5>Cody Lan</h5>
          <p>{{$t('team.team2')}}-{{$t('team.team3')}}</p>
        </li>
        <li class="fl">
          <h6><img src="./../assets/team/Wave-Tan.jpg"></h6>
          <h5>Wave Tan</h5>
          <p>{{$t('team.team16')}}-{{$t('team.team3')}}</p>
        </li>
        <li class="fl">
          <h6><img src="./../assets/team/WechatIMG212.jpeg"></h6>
          <h5>Lijun Zhou</h5>
          <p>{{$t('team.team2')}}-{{$t('team.team3')}}</p>
        </li>
        <li class="fl">
          <h6><img src="./../assets/team/Charlie-Li.jpg"></h6>
          <h5>Charlie Li</h5>
          <p>{{$t('team.team9')}}-{{$t('team.team3')}}</p>
        </li>
        <li class="fl">
          <h6><img src="./../assets/team/Pierre-Luo.jpg"></h6>
          <h5>Pierre Luo</h5>
          <p>{{$t('team.team2')}}-{{$t('team.team3')}}</p>
        </li>
        <li class="fl">
          <h6><img src="./../assets/team/ViVi-zhou.jpg"></h6>
          <h5>ViVi Zhou</h5>
          <p>{{$t('team.team2')}}-{{$t('team.team3')}}</p>
        </li>
        <li class="fl">
          <h6><img src="./../assets/team/Albert-Yi.jpg"></h6>
          <h5>Albert Yi</h5>
          <p>{{$t('team.team17')}}-{{$t('team.team3')}}</p>
        </li>
        <li class="fl">
          <h6><img src="./../assets/team/Angang-Tang.jpg"></h6>
          <h5>Angang Tang</h5>
          <p>{{$t('team.team9')}}-{{$t('team.team3')}}</p>
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
        width: 22rem;
        margin: 50px auto 100px;
        font-size: 48px;
        font-weight: 700;
        padding-bottom: 1.4rem;
        border-bottom: 0.4rem solid #1a56a4;
      }
      .fast {
        color: #ffffff;
        border-bottom: 0;
        @media screen and (max-width: 1520px) {
          color: #608FFF;
          border-bottom: 0.4rem solid #1a56a4;
        }
      }
      ul {
        li {
          margin: 0 4rem 5rem 0;
          @media screen and (max-width: 1520px) {
            margin: 0 1rem 3rem 0;
          }
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
              @media screen and (max-width: 1520px) {
                max-width: 17rem;
              }
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
            @media screen and (max-width: 1520px) {
              font-size: 1.2rem;
            }
          }
        }
      }
    }
  }
</style>
