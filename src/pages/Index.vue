

<template>
  <div class="index">
    <!-- top start -->
    <Top message="首页" />
    <!-- banner -->
    <Swiper/>
    <!-- contain start -->
    <main>
        <Gao/>
        <Copy/>
        <!-- <Pro/>  -->
    </main>
    <!-- foot start -->
    <Fot/>
  </div>
</template>


<script>
import Vue from "vue";
import VueAwesomeSwiper from "vue-awesome-swiper";
// 顶部组件
import Top from "@/components/Top";
// 轮播组件
import Swiper from "@/components/Swiper";
// 内容组件
import Gao from "@/components/Content";
//版权组件
import Copy from "@/components/Copyright";
// 产品组件
import Pro from "@/components/Product";
// 底部导航
import Fot from "@/components/Foot";

Vue.use(VueAwesomeSwiper);
import { swiper, swiperSlide } from "vue-awesome-swiper";
export default {
  name: "carrousel",
  // 轮播图片
  data() {
    return {
     
    };
  },

  // 定义子组件名称
  components: {
    Top: Top,
    Gao: Gao,
    Copy: Copy,
    Pro: Pro,
    Fot: Fot,
    Swiper: Swiper
  }
};
</script>
<style>
    *{
        margin: 0;
        padding: 0;
    }
    ul {
      list-style: none;
    }
</style>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped>

h1,
h2 {
  font-weight: normal;
}
a {
  color: #42b983;
}
.swp {
  margin-top: 20%;
}
.banner img {
  width: 100%;
  height: 100%;
  background: red;
  background-size: contain;
}
main {
  margin-bottom: 20%;
}

</style>

