<template>
  <div id="login" class="login" :style="{height:DocHeight+'px'}">
    <div class="container-fluid">
      <login-reg 
	      title="登录" 
	      placeholderUser="请输入账号" 
	      placeholderPsw="请输入密码" 
	      placeholderCode="请输入验证码" 
	      btnText="登录" 
	      @btnSubmit="btnSubmit"  
	      lesgo="去注册"
      >
      </login-reg>
    </div>
  </div>
</template>

<script>
// 通过import的方式导入
import loginReg from "@/components/loginReg/loginReg.vue";
export default {
  name: "login",
  components: {//注册组件
    loginReg,
  },
  data() {
    return {};
  },
  methods: {
    btnSubmit(data) {//接收子组件发送过来的事件/数据
      console.log(data);
    },
  }
}