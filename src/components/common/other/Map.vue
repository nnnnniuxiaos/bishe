<template>
  <div class="box">
    <div id="container" style="width:500px; height:300px"></div>
  </div>
</template>

<script>
import AMap from 'AMap' // 引入高德地图
export default {
  mounted () {
    this.init()
  },
  methods: {
    init () {
      let map = new AMap.Map('container', {
        center: [116.397428, 39.90923],
        resizeEnable: true,
        zoom: 10
      })
    }
  }
}
</script>