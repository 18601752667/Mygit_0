<template>
  <div class="root-container">
    <Header></Header>
    <div class="title"><span>客服中心</span></div>
    <Contact :content="contact"></Contact>
    <Consult :content="consult"></Consult>
    <Footer/>
  </div>
</template>

<script>
import Header from "@/components/CHVersion/Header";
import Contact from "@/components/CHVersion/header/customerServiceCenter/Contact";
import Consult from "@/components/CHVersion/header/customerServiceCenter/Consult";
import Footer from "@/components/CHVersion/Footer";

export default {
  name: "CustomerServiceCenter",
  components: {
    Header,
    Contact,
    Consult,
    Footer,
  },

  data() {
    return {
      contact: {
        title: "联系我们",
        companyName_ch: "上海鉴真信息科技有限公司",
        phone: "",
        email: "",
        companyWeb: "",
        companyAddress: "",
        postcode: ""
      },
      consult: {
        title: "留言板",

      }
    }
  }
}
</script>

<style scoped>
.root-container {
  width: 1180px;
  margin: 0 auto;
}
.title {
  width: 100%;
  display: block;
  height: 30px;
  line-height: 30px;
  color: #b3e8e8;
  text-align: center;
  font-size: 16px;
  background-color: #a90000;
}
.title span {
  display: block;
  width: 120px;
  margin: auto;
}
</style>