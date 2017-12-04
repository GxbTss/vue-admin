<template>
    <div class="login">
        <div class="login-container">
            <h3 class="title">后台管理系统</h3>
            <el-form ref="ruleForm" :model="ruleForm" :rules="rules">
                <el-form-item prop="username">
                    <el-input type="text" v-model="ruleForm.username" placeholder="请输入用户名"></el-input>
                </el-form-item>
                <el-form-item prop="password">
                    <el-input type="password" v-model="ruleForm.password" placeholder="请输入密码"></el-input>
                </el-form-item>
                <el-form-item>
                    <el-button type="primary" class="login-sub" @click.native.prevent="FormLogin('ruleForm')" :loading="loading">登陆</el-button>
                </el-form-item>
            </el-form>
        </div>
    </div>
</template>

<script>
  export default {
    data () {
      return {
        ruleForm: {
          username: '',
          password: ''
        },
        rules: {
          username: [
            {required: true, message: '请输入用户名', trigger: 'blur'}
          ],
          password: [
            {required: true, message: '请输入密码', trigger: 'blur'}
          ]
        },
        loading: false
      }
    },
    methods: {
      FormLogin (formName) {
        this.$refs[formName].validate((valid) => {
          if (valid) {
            this.loading = true
            setTimeout(() => {
              this.loading = false
            }, 2000)
          } else {
            this.$notify.error({
              title: '错误',
              message: '请输入正确的用户名和密码',
              offset: 100
            })
            return false
          }
        })
      }
    }
  }
</script>

<style lang="less" scoped>
    .login{
        position: relative;
        width: 100%;
        height: 100vh;
        background-color: #2d3a4b;
        color: #fff;
        &-container{
            position: absolute;
            left: 50%;
            top: 50%;
            margin-top: -200px;
            margin-left: -150px;
            width: 300px;
        }
        .title{
            font-size: 26px;
            margin-bottom: 20px;
            text-align: center;
        }
        &-sub{
            width: 100%;
        }
    }
</style>
