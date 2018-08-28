<template>
  <div class="home" >
<body background="/static/BackGround/bk27.jpg"
style=" background-repeat:no-repeat ;
background-size:100% 100%;
background-attachment:fixed;" >
			<br/>
			<br/>
      <br/>
      <br/>
      <br/>
			<span class="title">电子信息与通信学院分团委学生会</span>
			<br/>
			<br/>
		  <br/>
      <br/>
      <br/>
      <br/>
			<p>简称电信学院团协联，始于1960。</p>
      <p>电信学院各项学生活动的发起者、组织者，</p>
      <p>学生自己的群众性组织，</p>
      <p>是提倡自我教育、自我管理、自我服务，</p>
			<p>并为电信学院在校学生提供无偿服务的组织。</p>
				<br/><br/><br/><br/><br/><br/>
      <div class="footer-link">
					<p>Copyright © 2018 Institute of electronic</p>
          <p> information and communication </p>     
          <p>- Design: Association of science and technology</p>
			</div>
      <br/><br/><br/>
    </body>
  </div>
</template>
<script>
  export default {
    name: "home",
    data(){
      return{
        activeIndex:'1',
      };
    }
  }
</script>

<style scoped>
		div{font-family: "微软雅黑";width: 100%;height: 100%;margin: auto;text-align: center;color: #F5F5F5;}
      body{
    width: 100%;
  }
  .demo-ruleForm{
    margin-right: 6%;
    margin-left: 0;
  }
  .title{
    font-size: 1.5rem;
  }
  @media all and (min-width: 400px)and (max-width: 560px){
    .demo-ruleForm{
      margin-right: 15%;
      margin-left: 5%;
    }
    .title{
      font-size: 2rem;
    }

  }
  @media all and (min-width: 560px)and (max-width: 900px){
    .demo-ruleForm{
      margin-right: 22%;
      margin-left: 16%;
    }
    .title{
      font-size: 2.5rem;
    }
  }
  @media all and (min-width: 900px){
    .demo-ruleForm{
      margin-right: 30%;
      margin-left: 25%;
    }
    .title{
      font-size: 3rem;
    }
  }

</style>
