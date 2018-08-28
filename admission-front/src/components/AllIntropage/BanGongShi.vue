<template>
  <div>
    <body background="/static/BackGround/bk28.jpg" style=" background-repeat:no-repeat ;background-size:100% 100%;background-attachment:fixed;">
    <el-button icon="el-icon-back" v-on:click="handleCard('AllDepintro')"></el-button>
      <el-card :body-style="{ padding: '0px' }"  class="card" >
        <div>
			    <section>
			       <h3>办公室职能</h3>
		           <p>&emsp;管理</p>
               <p>&emsp;管理公用房，审核借用者的申请并合理<br/>&emsp;安排使用时间</p>
		           <p>&emsp;协助</p>
              <ul>
                  <li>协助主席团如开学生会例会，做好会议记录</li>
                  <li>协助主席团制定学生会工作计划，做好工作总结</li>
                  <li>协调监督各部门，完成各项活动的部门考核，协助主席团进行优秀部长和优秀部员的评选</li>
                </ul>
                <p>&emsp;发布</p>
                <ul>
                  <li>上传下达，执行主席团决议，监督各职能部门工作的展开情况并及时向主席团汇报</li>
                  <li>以学生会的名义发布重大事项的布告、通告。</li>
                </ul>
		      </section>
          <p>More Messages --<a href="http://mp.weixin.qq.com/s?__biz=MzA5Mjk1OTM2OA==&mid=2652256134&idx=1&sn=4ae2f92d363624907fb50bb906d91e07&chksm=8b87b061bcf03977b5d2a95c18885928af017c219239aac3318d2ab1de536c9b222da0e960bf&mpshare=1&scene=23&srcid=0828Y1GcI2QDO5ODzQsy4slk#rd" 
          target="_blank" >办公室部门介绍</a></p>
	    </div><br/>
      </el-card>
      <br/><br/><br/><br/><br/><br/><br/><br/><br/><br/><br/><br/><br/>
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
