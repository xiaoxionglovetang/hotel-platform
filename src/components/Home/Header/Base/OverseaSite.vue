<template>
  <div class="icon-container">
      <span class="iconfont">&#xe693;</span>
  </div>
</template>

<script>
export default {

}
</script>
<style lang="less" scoped>
@import (reference) '../../../../../static/css/base.less';
.icon-container {
  margin: 0 4px 0 4px;
  text-align: center;
}

.iconfont {
  .f-color-size(#666, 24px);
    &:hover {
    color: @primary-color;
    cursor: pointer;
  }
}
</style>
