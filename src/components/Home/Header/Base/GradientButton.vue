<template>
  <div>
    <a class="register-btn">注册</a>
  </div>
</template>

<script>
export default {

}
</script>

<style scoped lang="less">
@import (reference) '../../../../../static/css/base.less';

.register-btn {
  display: inline-block;
  .size(70px, 30px);
  border-radius: 3px;
  line-height: 30px;
  .f-color-size(#fff, 14px);
  text-align: center;
  background-color: @primary-button-color;
  &:hover {
    background-color: @primary-button-hover;
  }
}
</style>
