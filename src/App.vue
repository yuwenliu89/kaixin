<style>
::-webkit-scrollbar {
        display: none;
      }
#app{
  width:100%;
  height: 100vh;
  position: relative;
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
.an{
  color:rgb(18, 152, 205);
}
.s{
  width:100%;
  height:74vh;
  overflow-y: scroll;
  background-color: white;
}
.tian{
  width:300px;
  height:150px;
  margin: auto;
  border-radius: 15px;
  background-color: rgba(87,89,96);
  position: sticky;
  top: -20vh;
  z-index: 0.5;
  margin-top: 5px;
}
.tian div:nth-child(1){
  width:100%;
  height:40px;
}
.tian div:nth-child(1) img{
  width:20px;
  height:20px;
  margin-left: 10px;
  margin-top: 10px;
  float: left;
}
.tian div:nth-child(1) p:nth-child(2){
  width:80px;
  float: left;
margin-top: 10px;
margin-left: 5px;
text-align: center;
color:white;
}
.tian div:nth-child(1) span{
  float: left;
  margin-top: 10px;
  font-size: 14px;
  color:rgba(194, 190, 190);
}
.tian div:nth-child(1) p:last-child{
  float: right;
  margin-top: 10px;
  width:40px;
  font-size: 14px;
  border-radius: 5px 0 0 5px;
  border: 0.2px solid rgb(194, 190, 190);
  color:white;
}
.tian div:nth-child(2){
  width:100%;
  height:160px;
} 
.tian div:nth-child(2) img{
  width:75px;
  height:100px;
  margin-top: 2px;
  margin-left: 15px;
}
.tian div:nth-child(2) P{
  width:15px;
  height:40px;
  margin-top: 25px;
  float: right;
  color:white;
  font-size: 14px;
}
.tian div:nth-child(2) span{
  float: right;
  margin-top: 35px;
  color:rgb(194, 190, 190);
}
</style>

<template>
  <div id="app">
    <TouBu msg="Welcome to Your Vue.js App" />

    <div class="s">
      
      <div class="tian">
        <div>
          <img src="../账号.png">
          <p>微信用户</p>
          <span>体验卡今日到期</span>
          <p>反馈</p>
        </div>
        <div>
          <img src="https://weread-1258476243.file.myqcloud.com/weread/cover/40/3300012940/t4_3300012940.jpg">
          <span>></span>
          <p>书架</p>
            
        </div>
      </div>
      <div class="wu">
        <ul @click="fun($event)">
          <li @click="changeComponent('TuiJian')" class="an">推荐</li>
          <li  @click="changeComponent('FenLei')">分类</li>
          <li  @click="changeComponent('HelloWorld')">排行</li>
          <li  @click="changeComponent('NeiRon')">文学艺术</li>
          <li  @click="changeComponent('NeiRons')" >哲学社科</li>
        </ul>
      </div>
      <TuiJian v-if="currentComponent === 'TuiJian'" msg="Welcome to Your Vue.js App" />
      <HelloWorld v-if="currentComponent === 'HelloWorld'" msg="Welcome to Your Vue.js App" />
      <NeiRons v-if="currentComponent === 'NeiRons'" msg="Welcome to Your Vue.js App" />
      <NeiRon v-if="currentComponent === 'NeiRon'" msg="Welcome to Your Vue.js App" />
      <FenLei v-if="currentComponent === 'FenLei'" msg="Welcome to Your Vue.js App" />
      
    </div>
    
   
      <DiBu msg="Welcome to Your Vue.js App" />
  
  </div>
 
</template>
<script src="./main.js"></script>
<script>
import TouBu from './components/TouBu.vue' 
import TuiJian from './components/TuiJian.vue'
import HelloWorld from './components/HelloWorld.vue' 
 import NeiRon from './components/NeiRon.vue'
 import NeiRons from './components/NeiRons.vue'
 import DiBu from './components/DiBu.vue' 
 import FenLei from './components/FenLei.vue' 

 export default {
  name: 'App',
  components: {
    HelloWorld,
    TouBu,
    DiBu,
    TuiJian,
    NeiRon,
    NeiRons,
    FenLei,
  },
  data() {
  return {
    currentComponent: 'TuiJian',
    an:"an",
  };
},
methods: {
  changeComponent(componentName ) {
    this.currentComponent = componentName;
  },
  fun(item){
    console.log();
    let ta = event.target
    let ans = event.target.innerHTML
    let wen = document.querySelectorAll("li")
    wen[0].classList.remove(this.an)
    wen[1].classList.remove(this.an)
    wen[2].classList.remove(this.an)
    wen[3].classList.remove(this.an)
    wen[4].classList.remove(this.an)
    switch (ans) {
      case "推荐":
      ta.classList.add(this.an)
        break;
        case "分类":
      ta.classList.add(this.an)
        break;
        case "排行":
      ta.classList.add(this.an)
        break;
        case "文学艺术":
      ta.classList.add(this.an)
        break;
        case "哲学社科":
      ta.classList.add(this.an)
        break;
    }
  }
},
}

</script>

