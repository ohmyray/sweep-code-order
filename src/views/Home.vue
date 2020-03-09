<template>
  <div class="home">
    <!-- 骨架屏 -->
    <van-skeleton title
                  avatar
                  :row="3"
                  :loading="loading"></van-skeleton>

    <!-- header导航 -->
    <Header></Header>

    <!-- 各类导航 -->
    <Nav :icon="icons"></Nav>

    <!-- 猜你喜欢 -->
  </div>
</template>

<script>

import Header from '@/components/Home/header'
import Nav from '@/components/Home/navs'
export default {
  name: 'Home',
  components: {
    Header,
    Nav
  },
  data () {
    return {
      loading: true,
      // nav 图标
      icons: [
        {
          icon: 'icon-meishi',
          bg: '#FD9D21',
          url: '#',
          text: '美食'
        },
        {
          icon: 'icon-KTV',
          bg: '#8A90FA',
          url: '#',
          text: '美食'
        },
        {
          icon: 'icon-zhoubianyou',
          bg: '#FED030',
          url: '#',
          text: '美食'
        },
        {
          icon: 'icon-waimai',
          bg: '#FD9D21',
          url: '#',
          text: '美食'
        },
        {
          icon: 'icon-jiudian',
          bg: '#FD9D21',
          url: '#',
          text: '美食'
        },
        {
          icon: 'icon-xiuxian',
          bg: '#FED030',
          url: '#',
          text: '美食'
        },
        {
          icon: 'icon-dianzimaoyan-',
          bg: '#FF6767',
          url: '#',
          text: '猫眼'
        },
        {
          icon: 'icon-liren',
          bg: '#FF80C2',
          url: '#',
          text: '美食'
        },
        {
          icon: 'icon-meishi',
          bg: '#FD9D21',
          url: '#',
          text: '小吃快餐'
        },
        {
          icon: 'icon-qita',
          bg: '#00D3BE',
          url: '#',
          text: '全部分类'
        }
      ]
    }
  },
  mounted () {
    this.loading = false
  }
}
</script>
