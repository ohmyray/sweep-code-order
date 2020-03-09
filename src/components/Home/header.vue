<template>
  <div class="header">
    <div class="address">广州</div>
    <div class="search">
      <div class="content">
        <van-icon name="search" />
        请输入商家名、品类或者商圈……
      </div>
    </div>
    <div class="user">
      <van-icon name="user-circle-o" />
    </div>
  </div>
</template>

<script>
export default {

}
</script>

<style lang="less" scoped>
.header {
  height: 3.125rem;
  background-color: #ffce00;
  display: flex;
  padding: 0 1rem;
  box-sizing: border-box;
  align-items: center;
}
.address {
  width: 3.5rem;
  font-size: 0.9rem;
  &::after {
    content: '';
    display: inline-block;
    height: 0;
    width: 0;
    border: 0.4rem solid transparent;
    border-top: 1px solid #000;
    border-right: 1px solid #000;
    transform: rotate(135deg);
    position: absolute;
    top: 1.2rem;
    margin-left: 0.5rem;
  }
}

.search {
  flex: 1;
  display: flex;
  align-items: center;
  height: 100%;
  .content {
    flex: 1;
    display: flex;
    padding: 0.5rem;
    border-radius: 0.3rem;
    background-color: rgba(255, 255, 255, 0.9);
    font-size: 0.5rem;
    color: #ccc;
    .van-icon-search {
      font-size: 0.9rem;
    }
  }
}
.user {
  font-size: 1.4rem;
  margin-left: 1rem;
}
</style>
