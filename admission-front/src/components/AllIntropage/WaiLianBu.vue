<template>
  <div>
    <body background="/static/BackGround/bk28.jpg">
    <el-button icon="el-icon-back" v-on:click="handleCard('AllDepintro')"></el-button>
      <el-card :body-style="{ padding: '0px' }"  class="card" >
        <div>
          <section>
            <h3>一.工作简介</h3>
            <ul>外联部的工作相对其他部的工作来说比较特殊，我们的工作要走在其他部门之前，很需要其他部门的配合和提前得到各部门的协助，所以我们与其他部门搞好关系是非常必要的。外联部将会尽可能的发挥本部作用，与有可能成为合作伙伴的各企业，事业单位做好沟通与交流，建立良好的合作关系，以便为我系的各大活动提供物资所需，保障活动的完善与到位。
            </ul>
            <h3>二.工作内容</h3>
            <li>代表学校与各大院校保持及时的交流与沟通</li>
            <li>与和学校联系紧密的各机关单位保持良好的联系</li>
            <li>负责在学生会各大活动完成礼宾接待工作</li>
            <h3>三.招新要求</h3>
            <ul>外联部是最能体现其实践能力的团队，要求具有较高的综合素质。外联部对外代表着学生会乃至学校的形象，因此，外联部员在搞各项活动的过程中应尽量在校内外树立诚实守信，精练能干的形象，我们应以培养个人素质的的基础工作做起，并与各部保持密切联系。</ul>
		      </section>
        </div>
        <p>More Messages --<a href="http://mp.weixin.qq.com/s?__biz=MzA5Mjk1OTM2OA==&mid=2652256186&idx=1&sn=1a8f8040dc5c303d3d71c54fc63d7e56&chksm=8b87b05dbcf0394bdbb9280473a4e486e04aa1700e47165a0d78c3cc9eec3298d7c080436da8&mpshare=1&scene=23&srcid=0828rkgfW2DI3cY9LQtZIyUF#rd" 
          target="_blank" >外联部部门介绍</a></p>
      </el-card>
      <br/><br/><br/><br/><br/><br/><br/><br/><br/>
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
  div{font-family: "微软雅黑"}
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
