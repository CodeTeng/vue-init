<template>
  <div style="color: #666;font-size: 14px;">
    <div style="padding-bottom: 20px">
      <b>欢迎你！{{ user.nickname }}</b>
    </div>
    <el-card>
      狂小腾！！！
      <el-divider />
      虎虎生威，虎年大吉
    </el-card>
    <div style="height: 1px; background: #ddd; margin: 20px 0"/>

    <el-row :gutter="30">
      <el-col :span="12">
        <div style="padding: 20px 0; font-size: 20px">后台管理系统</div>
        <div>
          这是一款专门针对后台管理系统设计的代码，代码简单，结构清晰，如果你是小白，一定不要错过哦！！！
        </div>
        <div class="m-10"><el-button type="danger"><i class="el-icon-coin"></i>QQ：2300858713</el-button></div>
        <div class="m-10"><el-button type="primary"><i class="el-icon-s-custom"></i>VX：15290654216</el-button></div>
        <div class="m-10">
          <el-button type="primary"><i class="el-icon-link"></i> <a style="color: #fff" href="https://github.com/CodeTeng/Background-authority-management-system">Github源码</a></el-button>
        </div>
      </el-col>
      <el-col :span="12">
        <div style="padding: 20px 0; font-size: 20px">技术栈</div>
        <el-row>
          <el-col :span="12" style="line-height: 30px">
            <div><b>后端</b></div>
            <div>SpringBoot2</div>
            <div>Hutool</div>
            <div>Poi</div>
            <div>Lombok</div>
            <div>Mybatis/Mybatis-plus</div>
            <div>Spring</div>
            <div>SpringMVC</div>
            <div>Redis</div>
          </el-col>
          <el-col :span="12" style="line-height: 30px">
            <b>前端</b>
            <div>Vue2</div>
            <div>Vue-Router</div>
            <div>VueX</div>
            <div>ElementUI</div>
            <div>Axios</div>
          </el-col>
        </el-row>
      </el-col>
    </el-row>

    <el-row>
      <el-col :span="6">
        <el-card>
          <div slot="header" class="clearfix">
            <span>喝杯咖啡</span>
            <div style="text-align: center">
              <img src="../assets/zhifu.png" alt="">
              <div class="pd-10">您可以请作者喝杯咖啡以资鼓励</div>
            </div>
          </div>
        </el-card>
      </el-col>
    </el-row>
  </div>
</template>

<script>
export default {
  name: "Home",
  data() {
    return {
      user: localStorage.getItem("user") ? JSON.parse(localStorage.getItem("user")) : {}
    }
  }
}
</script>
