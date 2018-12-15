<template>
  <div class="header">
    <div class="header-left">
      <div class="iconfont back-icon" @click="handleClick">&#xe624;</div>
    </div>
    <div class="header-input">
      <span class="iconfont">&#xe632;</span>
      输入城市经典/游玩主题
    </div>
    <div class="header-right">
      城市
      <span class="iconfont arrow-icon">&#xe64a;</span>
    </div>
  </div>
</template>

<script>
export default {
  name: 'HomeHeader',
  methods: {
    handleClick: function () {
      alert('1')
    }
  }
}
</script>

<style lang="stylus" scoped>
  @import '~@/assets/styles/varibles.styl'
  .header
    display :flex
    line-height :.86rem
    background :$bgColor
    color :#fff
    .header-left
      width :.64rem
      float :left
      .back-icon
        text-align: center
        font-size: .4rem
    .header-input
      flex :1
      background :#fff
      color :#000
      height :.64rem
      line-height :.64rem
      margin :.12rem 0 0 .2rem
      padding-left :0.2rem
      border-radius :.1rem
    .header-right
      width :1.24rem
      float :right
      text-align :center
</style>
