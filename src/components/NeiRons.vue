<style>
::-webkit-scrollbar {
        display: none;
      }
.shi{
    width:100%;
  height:35vh;
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
}
.liu img{
  width:70px;
  height:100px;
  float: left;
}
.liu h3{
  width:30px;
  height:100%;
  float: left;
  line-height: 100px;
  text-align: center;
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
        <h3>{{ index+1}}</h3>
        <img src="https://weread-1258476243.file.myqcloud.com/weread/cover/40/3300012940/t4_3300012940.jpg">
        <div class="a">
          <h4>{{ item.name }}</h4>
          <span>{{item.span}}</span>
          <span>{{item.span1}}<span style="color:red">{{item.span2}}</span></span>
        </div>
        <p><img src="../../账号.png">{{ item.num }}</p>
    </div>
</div>
  </template>
<script>
export default({
    data(){
        return{
            i:0,
            arr:[
      {
        name:"置身事内:中国政府与经济发展兰小欢",
        img:"",
        span:"兰小欢",
        span1:"推荐值96.4%",
        span2:"好评如潮",
        num:132,
        i:this.i++,
      },
      {
        name:"纳瓦尔宝典",
        img:"",
        span:"埃里克·乔根森",
        span1:"推荐值83.3%",
        span2:"好评如潮",
        num:132,
        i:this.i++
      },
      {
        name:"富爸爸穷爸爸(20周年修订版)",
        img:"",
        span:"罗伯特·清崎",
        span1:"推荐值83.1%",
        span2:"好评如潮",
        num:132,
        i:this.i++
      },
      {
        name:"资本的秘密",
        img:"",
        span:"赫尔南多·德·索托",
        span1:"推荐值83.8%",
        span2:"好评如潮",
        num:132,
        i:this.i++
      },
      {
        name:"芒格之道",
        img:"",
        span:"查理·芒格 芒格书院",
        span1:"推荐值93.7%",
        span2:"好评如潮",
        num:132,
        i:this.i++
      },
      {
        name:"告别百年激进",
        img:"",
        span:"温铁军",
        span1:"推荐值92.6%",
        span2:"好评如潮",
        num:132,
        i:this.i++
      },
      {
        name:"如何开一家小而美的店",
        img:"",
        span:"陈国扩",
        span1:"推荐值90.5%",
        span2:"好评如潮",
        num:132,
        i:this.i++
      },
      {
        name:"原则",
        img:"",
        span:"瑞·达利欧",
        span1:"推荐值82.0%",
        span2:"好评如潮",
        num:132,
        i:this.i++
      },
      {
        name:"芯片战争",
        img:"",
        span:"余盛",
        span1:"推荐值93.8%",
        span2:"好评如潮",
        num:132,
        i:this.i++
      },
      {
        name:"硅谷钢铁侠:埃隆·马斯克的冒险人生",
        img:"",
        span:"阿什利·万斯",
        span1:"推荐值79.7%",
        span2:"好评如潮",
        num:132,
        i:this.i++
      },
      {
        name:"国富论",
        img:"",
        span:"亚当·斯密",
        span1:"推荐值86.2%",
        span2:"好评如潮",
        num:132,
        i:this.i++
      },
      {
        name:"干法",
        img:"",
        span:"稻盛和夫",
        span1:"推荐值81.7%",
        span2:"好评如潮",
        num:132,
        i:this.i++
      },
      {
        name:"冯唐成事心法",
        img:"",
        span:"冯唐",
        span1:"推荐值80.8%",
        span2:"好评如潮",
        num:132,
        i:this.i++
      },
      {
        name:"一本书读懂财报",
        img:"",
        span:"肖星",
        span1:"推荐值93.3%",
        span2:"好评如潮",
        num:132,
        i:this.i++
      },
      {
        name:"史蒂夫·乔布斯传 (2014修订版)",
        img:"",
        span:"沃尔特·艾萨克森",
        span1:"推荐值91.3%",
        span2:"好评如潮",
        num:132,
        i:this.i++
      },
      {
        name:"活法",
        img:"",
        span:"稻盛和夫",
        span1:"推荐值85.7%",
        span2:"好评如潮",
        num:132,
        i:this.i++
      },
      {
        name:"股票投资入门、进阶与实战",
        img:"",
        span:"朱孜;王俊龙",
        span1:"推荐值89.5%",
        span2:"好评如潮",
        num:132,
        i:this.i++
      },
      {
        name:"卓有成效的管理者",
        img:"",
        span:"彼得·德鲁克",
        span1:"推荐值86.2%",
        span2:"好评如潮",
        num:132,
        i:this.i++
      },
      {
        name:"褚时健传",
        img:"",
        span:"周桦",
        span1:"推荐值90.0%",
        span2:"好评如潮",
        num:132,
        i:this.i++
      },
      {
        name:"原则: 应对变化中的世界秩序",
        img:"",
        span:"瑞·达利欧",
        span1:"推荐值90.6%",
        span2:"好评如潮",
        num:132,
        i:this.i++
      },
    ]
        }
    }
})
</script>