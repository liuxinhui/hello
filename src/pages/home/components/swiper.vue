<template>
  <div class="wrapper">
    <swiper :options="swiperOption">
      <swiper-slide v-for='item in swiperList' :key="item.id">
        <img :src="item.imgUrl">
      </swiper-slide>
      <div class="swiper-pagination" slot="pagination"></div>
    </swiper>
  </div>
</template>

<script>
export default {
  name: 'HomeSwiper',
  data () {
    return {
      swiperOption: {
        pagination: '.swiper-pagination',
        loop: true,
        autoplay: false,
        speed: 2000
      },
      swiperList: [{
        id: '0001',
        imgUrl: 'https://img1.qunarzz.com/vs_ceph_vs_tts/92b5cd40-a368-4739-854c-b9532eee03f7.jpg_r_640x420x90_f4efb6b8.jpg'
      }, {
        id: '0002',
        imgUrl: 'https://img1.qunarzz.com/p/tts5/1808/ad/12b3e866039f9102.jpg_r_640x420x90_8ad5982d.jpg'
      }]
    }
  }
}
</script>

<style lang="stylus" scoped>
  .wrapper >>> .swiper-pagination-bullet-active
    background: red
  .wrapper
    overflow: hidden
    width: 100%
    height: 0
    padding-bottom: 40%
    background: #eee
    .swiper-img
      width: 100%
</style>
