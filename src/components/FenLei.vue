<style>
::-webkit-scrollbar {
        display: none;
      }
.chao{
    width:100%;
    height:38vh;
    /* overflow-y: scroll; */
    background-color: white;
    z-index: 1;
}
.ba{
    width:90%;
    height:100px;
    background-color: gray;
    margin-left: 5%;
    border-radius: 20px;
    float: left;
    margin-top: 10px;
    z-index: 1;
    /* overflow-y: scroll; */
}
.ba img{
    width:70px;
    height:90px;
    float: right;
    margin-top: 5px;
    margin-right: 10px;
}
.ba h3{
    width:66%;
    height:40px;
    line-height: 40px;
    text-indent: 1em;
    float: left;
}
.ba span:nth-child(3){
    width:66%;
    height:20px;
    float: left;
    text-indent: 1em;
    font-size: 14px;
}
.ba span:nth-child(4){
    width:66%;
    height:20px;
    text-indent: 1em;
    float: left;
    font-size: 14px;
}
.ba span:nth-child(5){
    width:66%;
    height:20px;
    text-indent: 1em;
    float: left;
    font-size: 14px;
}
</style>
<template>
    <div class="chao">
    <div class="ba" v-for="(item,index) in arr" :key="index">
        <img src="https://weread-1258476243.file.myqcloud.com/weread/cover/40/3300012940/t4_3300012940.jpg">
        <h3>{{item.name}}</h3>
        <span>1.{{item.span}}</span>
        <span>2.{{item.span1}}</span>
        <span>2.{{item.span2}}</span>
    </div>
</div>
</template>
<script>
export default({
    data(){
        return{
            arr:[
                {
                    name:"精品小说",
                    span:"斗破苍穹",
                    span1:"剑来",
                    span2:"三体(全集)",
                },
                {
                    name:"历史",
                    span:"明朝那些事儿(全集)",
                    span1:"长安的荔枝",
                    span2:"商:殷周之变与华夏新生",
                },
                {
                    name:"文学",
                    span:"我与地坛",
                    span1:"红楼梦",
                    span2:"平凡的世界(全三册)",
                },
                {
                    name:"艺术",
                    span:"生活蒙太奇",
                    span1:"新摄影笔记",
                    span2:"你好生活",
                },
                {
                    name:"人物传记",
                    span:"邓小平时代",
                    span1:"毛泽东传(全6卷)",
                    span2:"苏东坡传(纪念典藏版)",
                },
                {
                    name:"哲学宗教",
                    span:".道德经",
                    span1:"次第花开(2017修订新版)",
                    span2:"传习录",
                },
                {
                    name:"计算机",
                    span:".Python编程: 从入门到实践",
                    span1:"wed前端",
                    span2:"网络是怎样连接的",
                },
                {
                    name:"社会文化",
                    span:"厌女(增订本)",
                    span1:"法治的细节",
                    span2:"快乐上等:女性怎样自在地活",
                },
                {
                    name:"个人成长",
                    span:"人性的弱点",
                    span1:"开心生活",
                    span2:"当下的力量(白金版)",
                },
                {
                    name:"经济理财",
                    span:"号身事内:中国政府与经济发展",
                    span1:"纳瓦尔宝典",
                    span2:"富爸爸穷爸爸(20周年修订版)",
                },
                
            ]
        }
    }
})
</script>