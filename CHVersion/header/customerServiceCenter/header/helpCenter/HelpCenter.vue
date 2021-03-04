<!-------------------------------------------------------------------------------------
//                             Copyright(c) 2020
//  All rights are reserved by East China Normal University.
//-------------------------------------------------------------------------------------
//  Abstract:
//		帮助中心页面组件
//-------------------------------------------------------------------------------------
//	History:
//    ·2021.02.22  刘邦威
//      根据旧版帮助中心进行整理。
//------------------------------------------------------------------------------------>
<!-------------------------------------------------------------------------------------
                                     组件模板设定
-------------------------------------------------------------------------------------->
<template>
  <div class="root-container">
    <Header></Header>
    <div class="title"><span>帮助中心</span></div>

    <el-container style="min-height: 600px">
      <el-aside class="leftMenu" style="" width="auto">
        <HCSideMenu content="hCSideMenu"></HCSideMenu>
      </el-aside>
      <el-main class="rightContent">
        <router-view/>
      </el-main>
    </el-container>

    <Footer/>
  </div>
</template>

<!-------------------------------------------------------------------------------------
                                 组件模板属性和行为描述
-------------------------------------------------------------------------------------->
<script>
import Header from "@/components/CHVersion/Header";
// import FrequentlyAskedQuestions from "@/components/CHVersion/header/helpCenter/FrequentlyAskedQuestions";
import Footer from "@/components/CHVersion/Footer";
import HCSideMenu from "@/components/CHVersion/header/helpCenter/HCSideMenu";

export default {
  name: "HelpCenter",
  components: {
    HCSideMenu,
    // FrequentlyAskedQuestions,
    Header,
    Footer,
  },

  data () {
    return {

    }
  }
}
</script>

<!-------------------------------------------------------------------------------------
                                 组件模板样式设定
-------------------------------------------------------------------------------------->
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


