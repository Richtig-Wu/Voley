

<template>
  <div class="fenlei clearfix">
    <ul class="clearfix">
      <li v-for="fl in FL">
        <a v-bind:href="fl.url" >
            <img v-bind:src="fl.sc" alt="">
        </a>
      </li>
    </ul>
  </div>
</template>

<script>
export default {
  data() {
    return {
      FL: [
        { url: "#", sc: require("../assets/zhuanjia.png") },
        { url: "#", sc: require("../assets/keshi.png") },
        { url: "#", sc: require("../assets/jiuyi.png") },
        { url: "#", sc: require("../assets/zaixian.png") },
        { url: "#", sc: require("../assets/yiyuan.png") },
        { url: "#", sc: require("../assets/tiyan.png") },
        { url: "#", sc: require("../assets/yibao.png") },
        { url: "#", sc: require("../assets/yuyue.png") }
      ]
    };
  }
};
</script>
<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped>
*{
    margin: 0;
}
ul {
  list-style: none;
}
.fenlei ul{
  padding: 0.5em;
  background: hsl(225, 33%, 95%);
}
.fenlei img {
  width: 45%;
  float: left;
  margin:2%;
}
.fenlei li:nth-child(2n){
  
}
/* 清除浮动 */
.clearfix {
  content: "";
  display: block;
  clear: both;
}

.clearfix {
  zoom: 1;
}
</style>
