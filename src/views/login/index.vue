<template>
  <div class="login-container">
      <!-- 卡片 -->
    <el-card class="login-box">
      <img src="../../assets/images/logo_index.png" alt="LOGO" />
    <!-- 表单 -->
      <el-form>
        <el-form-item>
          <el-input placeholder="请输入您的手机号"></el-input>
        </el-form-item>
        <el-form-item>
          <el-input placeholder="请输入您的短信验证码" style="width: 280px"></el-input>
          <el-button style="float: right">发送验证码</el-button>
        </el-form-item>
        <el-form-item>
            <el-checkbox v-model="checked"></el-checkbox>
            我已阅读并同意
            <el-link type="primary">隐私条款</el-link>和
            <el-link type="primary">用户许可</el-link>
        </el-form-item>
        <el-from-item>
          <el-button type="primary" style="width: 100%">登录</el-button>
        </el-from-item>
      </el-form>
    </el-card>
  </div>
</template>

<script>
export default {
  data () {
    return {
      checked: true
    }
  }
}
</script>

<style lang="less" scoped>
.login-container {
  width: 100%;
  height: 100%;
  position: absolute;
  left: 0;
  top: 0;
  background: url(../../assets/images/login_bg.jpg) no-repeat center / cover;

 .login-box {
     width: 450px;
     height: 350px;
     position: absolute;
     left: 50%;
     top: 50%;
     transform: translate(-50%, -50%);

    img {
        display: block;
        width: '200px';
        margin: 10px auto 30px;
    }
 }
}
</style>
