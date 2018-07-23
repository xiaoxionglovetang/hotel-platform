<template>
  <div>
    <h1 class="title"> {{ msg }} </h1>
  </div>
</template>

<script>
export default {
  data () {
    return {
      msg: 'this is home page'
    }
  }
}
</script>

<style scoped lang="less">
@import (reference) '../../static/css/base.less';
.title {
  .size(900px, 500px);
}
</style>
