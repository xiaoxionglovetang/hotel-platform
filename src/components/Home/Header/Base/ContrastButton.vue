<template>
  <div>
    <a class="login-btn">登录</a>
  </div>
</template>

<script>
export default {

}
</script>

<style scoped lang="less">
@import (reference) '../../../../../static/css/base.less';

.login-btn {
  display: inline-block;
  .size(70px, 28px);
  border-radius: 3px;
  border:1px solid @primary-border;
  line-height: 28px;
  .f-color-size(@primary-button-color, 14px);
  text-align: center;
  background-color: #fff;
  &:hover {
    color: #fff;
    border-color:  @primary-button-hover;
    background-color: @primary-button-hover;
  }
}
</style>
