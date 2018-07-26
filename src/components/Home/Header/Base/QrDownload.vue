<template>
  <div class="icon-container">
    <Poptip trigger="hover" placement="bottom-end">
      <i class="iconfont">&#xe692;</i>
      <div class="api" slot="content">
        <div class="app">
          <img src="../../../../../static/img/home/app.png">
          <p>扫一扫APP下载</p>
        </div>
        <div class="we-chat">
          <img src="../../../../../static/img/home/we-chat.png">
          <p>关注微信</p>
        </div>
        <i class="cut-off-rule"></i>
      </div>
    </Poptip>
  </div>
</template>

<script>
export default {
  data () {
    return {
    }
  }
}
</script>

<style scoped lang="less">
  @import (reference) "../../../../../static/css/base.less";
  .iconfont {
    .f-color-size(#666, 22px);
    &:hover {
      color: @primary-color;
      cursor: pointer;
    }
  }
  .api {
    position: relative;

      .cut-off-rule {
     .tl(0, 50%);
      .size(1px, 110px);
      background-color: #999;
      opacity: .3;
    }
  }

  .app, .we-chat {
    display: inline-block;
    overflow: hidden;
  }
  .app {
    position: relative;
    right: 21px;
    .size(115px, 119px);
    text-align: left;
    img {
      position: relative;
      top: -4px;
    }
    p {
      position: relative;
      top: -8px;
      width: 104px;
      padding-left: 4px;
      .f-color-size(#666, 14px);
    }
  }
  .we-chat {
    position: relative;
    left: 18px;
    .size(97px, 119px);
    text-align: right;
      p {
      position: relative;
      top: -2px;
      text-align: center;
      width: 104px;
      .f-color-size(#666, 14px);
    }
  }

  &/deep/ .ivu-poptip-popper {
    .ivu-poptip-inner {
      position: relative;
      left: 30px;
      .size(300px, 158px);
      padding: 20px 27px 20px 20px;
      .ivu-poptip-body {
        padding: 0 1px;
      }
    }
    .ivu-poptip-arrow {
      right: 5px;
    }
  }
</style>
