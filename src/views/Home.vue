<template>
  <div class="home">
    <div class="header">
      <header-nav></header-nav>
    </div>
  </div>
</template>

<script>
import HeaderNav from '../components/Home/Header/HeaderNav'
export default {
  components: {
    HeaderNav
  }
}
</script>

<style lang="less" scoped>
@import (reference) '../../static/css/base.less';
.home {
  width: 100%;
  background-color: #fff;
}
.header {
  min-width: 990px;
}
</style>
