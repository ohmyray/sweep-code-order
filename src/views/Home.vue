<template>
  <div class="home">
    <!-- 骨架屏 -->
    <van-skeleton title
                  avatar
                  :row="3"
                  :loading="loading"></van-skeleton>

    <!-- header导航 -->
    <Header></Header>
  </div>
</template>

<script>

import Header from '@/components/Home/header'
export default {
  name: 'Home',
  components: {
    Header
  },
  data () {
    return {
      loading: true
    }
  },
  mounted () {
    this.loading = false
  }
}
</script>
