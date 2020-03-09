<template>
  <div class="navs">
    <div :key="index"
         v-for="(item, index) of icon"
         class="item">
      <div class="circle"
           :style="{backgroundColor:item.bg}">
        <van-icon class="iconfont"
                  :class="item.icon" />
      </div>
      <span>{{item.text}}</span>
    </div>
  </div>
</template>

<script>
export default {
  props: {
    icon: {
      type: Array,
      default: () => { }
    }
  }

}
</script>

<style lang="less" scoped>
.navs {
  width: 100%;
  display: flex;
  flex-wrap: wrap;
  font-size: 0.8rem;
  color: #808080;
}

.item {
  height: 5.2rem;
  width: 20%;
  display: flex;
  align-items: center;
  justify-content: center;
  flex-direction: column;
  .circle {
    display: flex;
    align-items: center;
    justify-content: center;
    border-radius: 50%;
    width: 2.5rem;
    height: 2.5rem;
    margin-bottom: 0.3rem;
  }
  .iconfont {
    font-size: 2rem;
    color: #fff;
  }
}
</style>
