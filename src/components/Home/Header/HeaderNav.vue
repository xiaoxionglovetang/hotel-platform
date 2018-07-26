<template>
  <div class="container">
    <div class="content-nav">
      <div class="top">
        <em class="logo"></em>
        <div class="nav-box">
          <nav-list></nav-list>
        </div>
        <div class="use-enter">
          <contrast-button class="login"></contrast-button>
          <gradient-button class="register"></gradient-button>
        </div>
        <span class="split"></span>
        <div class="icon-box">
          <qr-download class="qr"></qr-download>
          <ask-questions class="ask"></ask-questions>
          <oversea-site class="site"></oversea-site>
        </div>
      </div>
    </div>
  </div>
</template>

<script>
import NavList from './NavList'
import ContrastButton from './Base/ContrastButton'
import GradientButton from './Base/GradientButton'
import AskQuestions from './Base/AskQuestions.vue'
import OverseaSite from './Base/OverseaSite'
import QrDownload from './Base/QrDownload'
export default {
  components: { NavList, ContrastButton, GradientButton, AskQuestions, OverseaSite, QrDownload },
  data () {
    return {
    }
  }
}
</script>

<style lang="less" scoped>
@import (reference) "../../../../static/css/base.less";

.container {
  .size(100%, 59px);
  background-image: url("../../../../static/img/home/bg_header_index_top.png");
}

.content-nav {
  .size(1178px, 44px);
  padding-top: 15px;
  margin: 0 auto;
}

.top {
  .clearFix();
  .size(100%, 30px);
  // logo
  .logo {
    .lf;
    .size(109px, 30px);
    background: url("../../../../static/img/base/sprite_logo.png") 1px -119px no-repeat;
  }
  // nav-box
  .nav-box {
    .lf;
    .size(526px, 29px);
    margin: 5px 0 0 50px;
  }
}

// login and register
.use-enter {
  .rt;
  .size(162px, 30px);
  text-align: right;
  .login {
    display: inline-block;
    margin: 0 5px;
  }
  .register {
    display: inline-block;
    margin-left: 5px;
  }
}
.split {
  .rt;
  .size(1px, 12px);
  margin: 9px 15px 0 5px;
  background-color: #a9a9a4;
}

.icon-box {
  .rt;
  width: auto;
  height: 30px;
  .ask, .site, .qr {
    display: inline-block;
    margin: 0 4px;
  }
}
</style>
