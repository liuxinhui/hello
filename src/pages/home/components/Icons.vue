<template>
  <div class="icons">
    <div class="icon">
      <div class="icon-img">
        <img class='icon-img-content' src="@/assets/images/icon.png" />
        <p class="icon-desc">热门景点</p>
      </div>
    </div>
    <div class="icon">
      <div class="icon-img">
        <img class='icon-img-content' src="@/assets/images/icon.png" />
        <p class="icon-desc">热门景点</p>
      </div>
    </div>
    <div class="icon">
      <div class="icon-img">
        <img class='icon-img-content' src="@/assets/images/icon.png" />
        <p class="icon-desc">热门景点</p>
      </div>
    </div>
    <div class="icon">
      <div class="icon-img">
        <img class='icon-img-content' src="@/assets/images/icon.png" />
        <p class="icon-desc">热门景点</p>
      </div>
    </div>
    <div class="icon">
      <div class="icon-img">
        <img class='icon-img-content' src="@/assets/images/icon.png" />
        <p class="icon-desc">热门景点</p>
      </div>
    </div>
    <div class="icon">
      <div class="icon-img">
        <img class='icon-img-content' src="@/assets/images/icon.png" />
        <p class="icon-desc">热门景点</p>
      </div>
    </div>
    <div class="icon">
      <div class="icon-img">
        <img class='icon-img-content' src="@/assets/images/icon.png" />
        <p class="icon-desc">热门景点</p>
      </div>
    </div>
    <div class="icon">
      <div class="icon-img">
        <img class='icon-img-content' src="@/assets/images/icon.png" />
        <p class="icon-desc">热门景点</p>
      </div>
    </div>
  </div>
</template>

<script>
export default{
  name: 'HomeIcons'
}
</script>

<style lang="stylus" scoped>
  @import '~styles/varibles.styl'
    .icons
      height :0
      overflow :hidden
      padding-bottom: 50%
      border :1px solid red
      .icon
        float :left
        width :25%
        padding-bottom :25%
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
</style>
