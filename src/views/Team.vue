<template>
  <div class="team">
    <div class="team-list w1200">
      <h3 class="tc fast">{{$t('team.team0')}}</h3>
      <ul class="tc">
        <li style="margin: 0">
          <h6><img src="./../assets/team/Berzeck.png"></h6>
          <h5>Berzeck</h5>
        </li>
      </ul>
    </div>
    <div class="cb"></div>
    <div class="team-list w1200">
      <h3 class="tc" style="margin-top: 120px">{{$t('team.team1')}}</h3>
      <p class="info">{{$t('team.team18')}}</p>
      <el-row :gutter="20" class="teams">
        <el-col :span="6"><h6><img src="./../assets/team/Moshe.png"></h6>
          <h5>Moshe</h5>
          <p>{{$t('team.team4')}}-{{$t('team.team5')}}</p></el-col>
        <el-col :span="6">
          <h6><img src="./../assets/team/Angel.png"></h6>
          <h5>Angel</h5>
          <p>{{$t('team.team4')}}-{{$t('team.team6')}}</p>
        </el-col>
        <el-col :span="6">
          <h6><img src="./../assets/team/Claudio.png"></h6>
          <h5>Claudio</h5>
          <p>{{$t('team.team7')}}-{{$t('team.team8')}}</p>
        </el-col>
        <el-col :span="6">
          <h6><img src="./../assets/team/Naveen.png"></h6>
          <h5>Naveen</h5>
          <p>{{$t('team.team9')}}-{{$t('team.team10')}}</p>
        </el-col>
        <el-col :span="6">
          <h6><img src="./../assets/team/nalex.jpeg"></h6>
          <h5>Nalex</h5>
          <p>{{$t('team.team11')}} - {{$t('team.team12')}}</p>
        </el-col>
        <el-col :span="6">
          <h6><img src="./../assets/team/Tudor.jpeg"></h6>
          <h5>Tudor</h5>
          <p>{{$t('team.team4')}}-{{$t('team.team12')}}</p>
        </el-col>
        <el-col :span="6">
          <h6><img src="./../assets/team/kathy.jpeg"></h6>
          <h5>Kathy</h5>
          <p>{{$t('team.team2')}}-{{$t('team.team15')}}</p>
        </el-col>
      </el-row>
    </div>
    <div class="cb"></div>
  </div>
</template>

<script>
  export default {
    name: 'team',
  }
</script>
<style lang="less">
  .team {
    height: 2400px;
    .team-list {
      h3 {
        width: 22rem;
        margin: 50px auto 50px;
        font-size: 48px;
        font-weight: 700;
        padding-bottom: 1.4rem;
        border-bottom: 0.4rem solid #1a56a4;
      }
      .fast {
        color: #ffffff;
        border-bottom: 0;
        @media screen and (max-width: 1770px) {
          color: #608FFF;
          border-bottom: 0.4rem solid #1a56a4;
        }
      }
      .info {
        margin: 0 0 100px 0;
      }
      .teams, ul {
        .el-col-6, li {
          margin: 0 0 5rem 0;
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
