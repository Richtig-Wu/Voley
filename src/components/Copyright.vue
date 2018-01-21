
<template>
    <div class="copy">
        <div class="links">
            <span>友情链接:</span>
            <ul>
                <li v-for="lin in links"><a v-bind:href="lin.url">{{lin.name}}</a></li>
            </ul>
        </div>
        <hr>
        <div class="copy-text">
          <p>
            东莞长安霄边医院版权所有
          </p>
          <p>
            医院地址: 东莞长安镇霄边大道1号(358省道旁) 邮编(523851)
          </p>
          <p>咨询热线: 0769-85531888 门诊时间: 8:00-20:00 全年节假日不休(开展夜间妇产科急诊)</p>
          <p>
            声明: 本站信息仅供参考,并不作为疾病诊疗依据。如果您想了解更多健康问题, 请点击<a href="http://p.qiao.baidu.com/cps/chat?siteId=11489345&userId=24818518">咨询在线医生</a>
          </p>
          <p>备案号:<a href="http://www.miitbeian.gov.cn">粤ICP备17038563号-2</a></p>
        </div>
    </div>
</template>


<script>
export default {
  data() {
    return {
      links: [
        { url: "https://www.baidu.com/", name: "百度" },
        { url: "https://nianhuo.tmall.com/", name: "天猫" },
        { url: "https://www.vip.com/", name: "唯品会" },
        { url: "https://www.github.com/", name: "Github" },
        { url: "https://translate.google.cn/", name: "Google翻译" },
        { url: "https://www.github.com/", name: "Github" },
        { url: "https://translate.google.cn/", name: "Google翻译" },
        { url: "https://www.github.com/", name: "Github" },
        { url: "https://translate.google.cn/", name: "Google翻译" },
        { url: "https://developer.mozilla.org/zh-CN/", name: "MDN" }
      ]
    };
  }
};
</script>
<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped>
hr {
  height: 0.1px;
  margin: 0;
  padding: 0;
  background: rgb(145, 145, 145);
}
.copy {
  background: #009ed9;
  padding-bottom: 5%;
}
.copy ul li {
  float: left;
  border: 1px solid #fff;
  border-radius: 0.2em;
  background: #4a85d1;
}
.copy a {
  color: #fff;
}
/* 友情链接css */
.links span {
  font-size: 1.2em;
  margin-left: 0.2em;
}
.links ul {
  display: flex;
  display: -webkit-flex;
  justify-content: space-around;
  flex-wrap: wrap;
}
.links ul li {
  margin-top: 0.5em;
  padding: 0.1px 0.5em;
}

/* copy-text */
.copy-text {
  margin: 1.8em 0;
}
.copy-text p {
  text-align: center;
  font-size: 1.1em;
  color: rgb(186, 227, 233);
}
.copy-text p a {
  color: black;
}
</style>