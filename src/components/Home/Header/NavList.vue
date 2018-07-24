<template>
  <ul class="list">
    <li :class="{'currently-clicked': isCurrentlyClicked === item.id}" v-for="item in items" :key="item.id" @click="onCurrentlyClicked(item.id)">{{ item.name }}</li>
  </ul>
</template>

<script>
export default {
  data () {
    return {
      items: [
        { id: '0', name: '首 页' },
        { id: '1', name: '国内酒店' },
        { id: '2', name: '海外酒店' },
        { id: '3', name: '特卖专区' },
        { id: '4', name: '旗下品牌' },
        { id: '5', name: '华住会' },
        { id: '6', name: '华住商旅' }
      ],
      isCurrentlyClicked: '0'
    }
  },
  methods: {
    onCurrentlyClicked (id) {
      this.isCurrentlyClicked = id;
    }
  }
}
</script>

<style scoped lang="less">
@import (reference) "../../../../static/css/base.less";
.list {
  .clearFix();
  margin: 0;
  padding-left: 0;
}

li {
  .lf;
  padding-bottom: 6px;
  margin-right: 19px;
  .f-color-size(@gray-three-color, 15px);
  opacity: 0.7;
  &:hover{
    color: @primary-color;
    opacity: 1;
    cursor: pointer;
    transition: color .2s;
  }
}

.currently-clicked {
  font-weight: bold;
  opacity: 1;
  .f-color-size(@primary-color, 16px);
}
</style>
