<style>
::-webkit-scrollbar {
        display: none;
      }
      li{
        list-style: none;
      }
*{
  margin: 0;
  padding: 0;
}
.box{
  width:100%;
  height:35vh;
  background-color: red;
}
.san{
  width:100%;
  height:35vh;
  background-color: white;
  margin: auto;
  margin-top: 20px;
  /* overflow-y: scroll; */
  position: relative;
}
.si{
  width:300px;
  height: 200px;;
  margin: auto;
  border-radius: 15px;
  background-color: rgba(87,89,96);
}
.wu{
  width:100%;
  height:40px;
  position: sticky;
  top: 0px;
  z-index: 5;
  background-color: white;
}
.wu ul{
  width:100%;
  height:30px;
}
.wu ul li{
  width:20%;
  height:30px;
  line-height: 30px;
  float: left;
  text-align: center;
  margin-top: 5px;
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
width:55%;
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
.qi{
  width:100%;
  background-color: white;
}

</style>
<template>
  <div class="box">

    <div class="san">
<!--       <div class="si">

      </div> -->
<!--       <div class="wu">
        <ul>
          <li @click="changeComponent('TuiJian')">推荐</li>
          <li  @click="changeComponent('FenLei')">分类</li>
          <li  @click="changeComponent('HelloWorld')">排行</li>
          <li  @click="changeComponent('NeiRon')">文学艺术</li>
          <li  @click="changeComponent('NeiRons')">哲学社科</li>
        </ul>
      </div> -->
      <div class="qi">
      <div class="liu" v-for="(item,index) in arr" :key="index">
        <h3>{{ index+1}}</h3>
        <img src="https://weread-1258476243.file.myqcloud.com/weread/cover/40/3300012940/t4_3300012940.jpg">
        <div class="a">
          <h4>{{ item.name }}</h4>
          <span>{{item.span}}</span>
          <span>{{item.span1}}<span style="color:red">{{item.span2}}</span></span>
        </div>
        <!-- <p><img src="../../账号.png">{{ item.num }}</p> -->
      </div>
    </div>
    </div>
    </div>
</template>

<script>
 export default{
  data(){
    return{
      i:0,
      currentComponent: 'HelloWorld',
    arr:[
      {
        name:"厌女（增订本）",
        img:"",
        span:"上野千鹤子",
        span1:"推荐值89.1%",
        span2:"好评如潮",
        num:132,
        i:this.i++,
      },
      {
        name:"法治的细节",
        img:"",
        span:"罗翔",
        span1:"推荐值93.9%",
        span2:"好评如潮",
        num:132,
        i:this.i++
      },
      {
        name:"乡土中国",
        img:"",
        span:"费孝通",
        span1:"推荐值85.5%",
        span2:"好评如潮",
        num:132,
        i:this.i++
      },
      {
        name:"始于极限:女性主义往复书简",
        img:"",
        span:"上野千鹤子 铃木凉美",
        span1:"推荐值90.6%",
        span2:"好评如潮",
        num:132,
        i:this.i++
      },
      {
        name:"枪炮、病菌与钢铁",
        img:"",
        span:"贾雷德·戴蒙德",
        span1:"推荐值87.3%",
        span2:"好评如潮",
        num:132,
        i:this.i++
      },
      {
        name:"小镇喧嚣:一个乡镇政治运作的演绎与阐释",
        img:"",
        span:"吴毅",
        span1:"推荐值96.2%",
        span2:"好评如潮",
        num:132,
        i:this.i++
      },
      {
        name:"圆圈正义:作为自由前提的信念",
        img:"",
        span:"罗翔",
        span1:"推荐值92.5%",
        span2:"好评如潮",
        num:132,
        i:this.i++
      },
      {
        name:"刑法学讲义(法律男神罗翔的刑法普及课)",
        img:"",
        span:"罗翔",
        span1:"推荐值93.4%",
        span2:"好评如潮",
        num:132,
        i:this.i++
      },
      {
        name:"从零开始的女性主义",
        img:"",
        span:"上野千鹤子 田房永子",
        span1:"推荐值90.7%",
        span2:"好评如潮",
        num:132,
        i:this.i++
      },
      {
        name:"娱乐至死",
        img:"",
        span:"尼尔·博斯曼",
        span1:"推荐值75.6%",
        span2:"好评如潮",
        num:132,
        i:this.i++
      },
      {
        name:"工作、消费主义和新穷人",
        img:"",
        span:"齐格蒙特、鲍曼",
        span1:"推荐值76.8%",
        span2:"好评如潮",
        num:132,
        i:this.i++
      },
      {
        name:"万古江河",
        img:"",
        span:"许停云",
        span1:"推荐值87.5%",
        span2:"好评如潮",
        num:132,
        i:this.i++
      },
      {
        name:"中国古代文化常识",
        img:"",
        span:"王力",
        span1:"推荐值91.2%",
        span2:"好评如潮",
        num:132,
        i:this.i++
      },
      {
        name:"最好的告别",
        img:"",
        span:"阿图·葛文德",
        span1:"推荐值86.6%",
        span2:"好评如潮",
        num:132,
        i:this.i++
      },
      {
        name:"山海经(全译插图典藏)",
        img:"",
        span:"小恐共",
        span1:"推荐值79.7%",
        span2:"好评如潮",
        num:132,
        i:this.i++
      },
      {
        name:"看不见的女性",
        img:"",
        span:"卡罗琳·克里亚多·佩雷斯",
        span1:"推荐值92.5%",
        span2:"好评如潮",
        num:132,
        i:this.i++
      },
      {
        name:"这里是中国",
        img:"",
        span:"星球研究所 中国青藏高原研究会",
        span1:"推荐值85.8%",
        span2:"好评如潮",
        num:132,
        i:this.i++
      },
      {
        name:"乡土中国",
        img:"",
        span:"费孝通",
        span1:"推荐值92.5%",
        span2:"好评如潮",
        num:132,
        i:this.i++
      },
      {
        name:"父权制与资本主义",
        img:"",
        span:"上野千鹤子",
        span1:"推荐值91.0%",
        span2:"好评如潮",
        num:132,
        i:this.i++
      },
      {
        name:"身为女性的选择",
        img:"",
        span:"上野千鹤子 信田小夜子",
        span1:"推荐值77.6%",
        span2:"好评如潮",
        num:132,
        i:this.i++
      },
    ],
  }
    },

methods: {
  changeComponent(componentName) {
    this.currentComponent = componentName;
  },
},

  }
</script>
