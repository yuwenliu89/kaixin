<style>
::-webkit-scrollbar {
        display: none;
      }
.shi{
    width:100%;
  height:65vh;
  background-color: white;
  margin: auto;
  margin-top: 20px;
  /* overflow-y: scroll; */
  position: relative;
}
.liu{
  width:100%;
  height:100px;
  margin-top:10px;
  position: relative;
  background-color: white;
}
.liu img{
  width:70px;
  height:100px;
  float: left;
  margin-left:15px;
}

.liu p{
  width:50px;
  height:20px;
  float: right;
  font-size: 13px;
  color:gray;
  text-align: center;
  border-radius: 10px;
  border:0.2px solid gray;
}
.liu p img{
  width:12px;
  height:12px;
  margin-top: 3px;
  margin-left:2px;
}
.a{
width:52%;
height:100px;
float: left;
margin-left:10px;
background-color: white;
}
.liu .a h4{
  width:100%;
  height:50px;
  text-align: left;
  font-size: 20px;
}
.a span:nth-child(2){
  width:100%;
  height:20px;
  float: left;
  font-size: 14px;
  color:gray;
}
.a span:nth-child(3){
  width:100%;
  height:20px;
  float: left;
  font-size: 14px;
  color:rgb(194, 190, 190);
}
</style>
<template>
<div class="shi">
  
    <div class="liu" v-for="(item,index) in arr" :key="index">
            <img src="https://weread-1258476243.file.myqcloud.com/weread/cover/40/3300012940/t4_3300012940.jpg">
        <div class="a">
          <h4>{{item.name}}</h4>
          <span>{{item.span}}|{{ item.span1 }}</span>
          <span style="color:red">{{item.span2}}</span>
        </div>
    </div>
</div>
</template>
<script>
export default({
    data(){
        return{
            arr:[
      {
        name:"剑来(1-42册)出版精校版",
        img:"",
        span:"烽火戏诸侯",
        span1:"推荐值80.8%",
        span2:"大家都在读",

      },
      {
        name:"长安的荔枝",
        img:"",
        span:"马伯庸",
        span1:"推荐值95.5%",
        span2:"大家都在读",


      },
      {
        name:"平凡的世界(全三册)",
        img:"",
        span:"路遥",
        span1:"推荐值93.1%",
        span2:"大家都在读",

      },
      {
        name:"认知觉醒:开启自我改变的原动力",
        img:"",
        span:"周岭",
        span1:"推荐值91.3%",
        span2:"大家都在读",

      },
      {
        name:"活着",
        img:"",
        span:"余华",
        span1:"推荐值91.9%",
        span2:"大家都在读",
 
      },
      {
        name:"三体(全集)",
        img:"",
        span:"刘慈欣",
        span1:"推荐值93.4%",
        span2:"大家都在读",

      },
      {
        name:"我与地坛",
        img:"",
        span:"史铁生",
        span1:"推荐值91.5%",
        span2:"大家都在读",
  
      },
      {
        name:"法医秦明:白卷",
        img:"",
        span:"法医秦明",
        span1:"推荐值89.9%",
        span2:"大家都在读",

      },
      {
        name:"蒋廷蔽中国近代史",
        img:"",
        span:"蒋廷懒 ",
        span1:"推荐值89.2%",
        span2:"大家都在读",

      },
      {
        name:"长安的荔枝",
        img:"",
        span:"马伯庸",
        span1:"推荐值95.5%",
        span2:"大家都在读",

      },
      {
        name:"我的前半生",
        img:"",
        span:"爱新觉罗·溥仪",
        span1:"推荐值80.4%",
        span2:"大家都在读",

      },
      {
        name:"认知觉醒:开启自我改变的原动力",
        img:"",
        span:"周岭",
        span1:"推荐值91.3%",
        span2:"大家都在读",
 
      },
      {
        name:"活着",
        img:"",
        span:"余华",
        span1:"推荐值91.9%",
        span2:"大家都在读",

      },
      {
        name:"余华作品全集(《活着》等13册)",
        img:"",
        span:"余华",
        span1:"推荐值88.8%",
        span2:"大家都在读",
 
      },
      {
        name:"我与地坛",
        img:"",
        span:"史铁生",
        span1:"推荐值91.0%",
        span2:"大家都在读",

      },
      {
        name:"剑来(1-42册)出版精校版",
        img:"",
        span:"烽火戏诸侯",
        span1:"推荐值80.8%",
        span2:"大家都在读",

      },
      {
        name:"长安的荔枝",
        img:"",
        span:"马伯庸",
        span1:"推荐值95.5%",
        span2:"大家都在读",


      },
      {
        name:"平凡的世界(全三册)",
        img:"",
        span:"路遥",
        span1:"推荐值93.1%",
        span2:"大家都在读",

      },
      {
        name:"认知觉醒:开启自我改变的原动力",
        img:"",
        span:"周岭",
        span1:"推荐值91.3%",
        span2:"大家都在读",

      },
      {
        name:"活着",
        img:"",
        span:"余华",
        span1:"推荐值91.9%",
        span2:"大家都在读",
 
      },
    ]
        }
    }
})
</script>