<template>
  <div class="icon-container">
    <Poptip trigger="hover" placement="bottom" width="130">
      <i class="iconfont">&#xe67f;</i>
      <ul class="api" slot="content">
        <li class="item" v-for="item in items" :key="item.id">
          <i class="iconfont icon" v-html="item.iconCode">{{ item.iconCode }}</i>
          <span class="name">{{ item.name }}</span>
        </li>
      </ul>
    </Poptip>
  </div>
</template>

<script>
export default {
  data () {
    return {
      items: [
        {iconCode: '&#xe648;', name: '华小二在线'},
        {iconCode: '&#xe60e;', name: '新手帮助'}
      ]
    }
  }
}
</script>

<style scoped lang="less">
  @import (reference) "../../../../../static/css/base.less";
  .iconfont {
    .f-color-size(#666, 23px);
    &:hover {
      color: @primary-color;
      cursor: pointer;
    }
  }
  .api {
    overflow: hidden;
    display: inline-block;
    min-height: 36px;
    .item {
      display: block;
      width: 128px;
      padding: 1px;
      .lh(30px);
      text-align: left;
      &:hover {
        cursor: pointer;
        background-color: rgba(153, 153, 153, 0.1);
        .icon {
          color: @primary-color;
        }
      }
      .icon, .name{
        display: inline-block;
        .lh(32px);
      }
      .icon {
        padding: 0 5px 0 10px;
        .f-color-size(#000, 18px)
      }
      .name {
        .f-color-size(#666; 14px);
        &:hover {
          color: @primary-color;
        }
      }
    }
  }
  // iView style
  &/deep/ .ivu-poptip-popper {
    min-width: 130px;
    .ivu-poptip-inner {
      width: 130px;
      padding: 8px 0;
      .ivu-poptip-body {
        padding: 0 1px;
      }
    }
  }
</style>
