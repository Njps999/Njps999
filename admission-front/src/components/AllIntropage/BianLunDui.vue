<template>
  <div>
    <body background="/static/BackGround/bk28.jpg">
    <el-button icon="el-icon-back" v-on:click="handleCard('AllDepintro')"></el-button>
      <el-card :body-style="{ padding: '0px' }"  class="card" >
        <div>
          <ul type="disc">
            <li>优秀的我们</li>
            <br>电信学院辩论队成立于2010年，是一支年轻的队伍，但实力却不容小觑。短短几年内，该队伍已经取得了喻晓亚军，新生杯亚军，喻晓四强这样的好成绩，以优秀的辩论成绩证明，电信饺子们不仅能做好技术，对辩论了同样在行<br>&emsp;
            <li>环境氛围</li>
            至于男女比~脱单率~队内氛围嘛……只能说，不能再好了！<br>（毕竟这是一个可以和全校各个年级的辩友聊人生谈理想顺便互留联系方式的正规组织嘛)<br>hohohohohohohoho!<br>&emsp;
            <li>辩论队给我们带来了什么？</li>
            <ul type="square">
              <li>更加清晰、系统的思路，更加敏捷的思维，更加全面的考虑问题的视角;</li>
              <li>更加广阔的知识面；（看着电脑里满满的论文嘿嘿一笑）</li>
              <li>倾听他人观点并快速总结、归纳、分析的能力，更好的临场反应能力;(若用于撩妹/撩汉，同学你的前途将一片光明)</li>
              <li>团队协作能力及口语交际能力；(每次的写稿都是一次博弈)</li>
              <section>
                <h3>最最最最重要的是........</h3>
                <p>你将收获超级丰富的课余生活，一群志同道合的好友，优秀的学长以及美丽的学姐（没错就是这样），还有大佬（辩论学习！）粗壮的大腿！</p>
                <h3>心动了吗？快来加入我们吧！</h3>
              </section>
		      	</ul>
		      </ul>
          </div>
          <p>More Messages --<a href="http://mp.weixin.qq.com/s?__biz=MzA5Mjk1OTM2OA==&mid=2652256184&idx=1&sn=e2749466bec3dc44cf292562e4669715&chksm=8b87b05fbcf039496f988c606065fa09ee87ba0f6e636a3fd34f376cce6aee7d0284ad0d92f3&mpshare=1&scene=23&srcid=0828F0oS7eZJtcWB8GoPTClD#rd" 
          target="_blank" >辩论队部门介绍</a></p>
      </el-card>
      <br/><br/><br/><br/>
    </body>
    </div>
</template>

<script>
  export default {
    name: "display",
    methods: {
      handleCard:function (key) {
        switch (key) {
          case 'AllDepintro':
            this.$router.push('/AllDepintro');
            break;
          default:
            this.$router.push('/Home');
        }
        console.log(key)
      }
  }
  }
</script>

<style scoped>
  .card{
    border-radius: 0;
    margin-left: 0;
    margin-right: 0;
    padding-left: 1rem;
    padding-right: 1rem;
    height: auto;
  }

  @media all and (min-width: 330px)and (max-width: 420px){
    .card{
      border-radius: 10px;
      margin-left: 16px;
      margin-right: 16px;
      padding-left: 1.5rem;
      padding-right: 1.5rem;
    }
  }

  @media all and (min-width: 420px)and (max-width: 800px){
    .card{
      border-radius: 20px;
      margin-left: 35px;
      margin-right: 35px;
      padding-left: 2rem;
      padding-right: 2rem;
    }
  }
  @media all and (min-width: 800px){
    .card{
      border-radius: 20px;
      margin-left: 60px;
      margin-right: 60px;
      padding-left: 2.5rem;
      padding-right: 2.5rem;
    }
  }

</style>
