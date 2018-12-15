<template>
  <div class="icons">
    <swiper :options="swiperOption">
      <swiper-slide v-for="(page, index) of pages" :key="index">
        <div
          class="icon"
          v-for="item of page"
          :key="item.id"
        >
          <div class="icon-img">
            <img class='icon-img-content' :src='item.iconsUrl' />
            <p class="icon-desc">{{item.title}}</p>
          </div>
        </div>
      </swiper-slide>
    </swiper>
  </div>
</template>

<script>
export default{
  name: 'HomeIcons',
  data () {
    return {
      swiperOption: {},
      iconsList: [{
        id: '00001',
        iconsUrl: 'https://pic.52112.com/icon/256/20170925/9240/512557.png',
        title: '热门景点热门景点'
      }, {
        id: '00002',
        iconsUrl: 'https://pic.52112.com/icon/256/20170928/9391/514752.png',
        title: '河北旅游'
      }, {
        id: '00003',
        iconsUrl: 'https://pic.52112.com/icon/256/20170928/9391/514752.png',
        title: '河北13'
      }, {
        id: '00004',
        iconsUrl: 'https://pic.52112.com/icon/256/20170928/9391/514752.png',
        title: '河北13'
      }, {
        id: '00005',
        iconsUrl: 'https://pic.52112.com/icon/256/20170928/9391/514752.png',
        title: '河北13'
      }, {
        id: '00006',
        iconsUrl: 'https://pic.52112.com/icon/256/20170928/9391/514752.png',
        title: '河北13'
      }, {
        id: '00007',
        iconsUrl: 'https://pic.52112.com/icon/256/20170928/9391/514752.png',
        title: '河北13'
      }, {
        id: '00008',
        iconsUrl: 'https://pic.52112.com/icon/256/20170928/9391/514752.png',
        title: '河北13'
      }, {
        id: '00009',
        iconsUrl: 'https://pic.52112.com/icon/256/20170928/9391/514752.png',
        title: 'handan'
      }]
    }
  },
  computed: {
    pages () {
      const pages = []
      this.iconsList.forEach((item, index) => {
        const page = Math.floor(index / 8)
        if (!pages[page]) {
          pages[page] = []
        }
        pages[page].push(item)
      })
      return pages
    }
  }
}
</script>

<style lang="stylus" scoped>
  @import '~styles/varibles.styl'
    .icons >>> .swiper-container
      height :0
      padding-bottom: 52%
      border :1px solid red
    .icon
      float :left
      width :25%
      padding-bottom :26%
      position :relative
      .icon-img
        position :absolute
        top: 0
        left :0
        right :0
        bottom :.44rem
        box-sizing :border-box
        padding :.1rem
        .icon-img-content
          border-radius :0.3rem
          display :block
          margin :0 auto
          width :1.5rem
        .icon-desc
          position: absolute
          left: 0
          right: 0
          bottom: 0
          top :1.6rem
          height: .44rem
          line-height: .44rem
          text-align: center
          color :$darkTextColor
          white-space: nowrap
          overflow: hidden
          text-overflow: ellipsis
</style>
