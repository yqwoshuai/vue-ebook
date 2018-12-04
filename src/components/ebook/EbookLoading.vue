<template>
  <div class="ebook-loading">
    <div class="ebook-loading-wrapper">
      <div class="ebook-loading-item">
        <div class="ebook-loading-line-wrapper">
          <div class="ebook-loading-line ebook-loading-line-01"></div>
        </div>
        <div class="ebook-loading-line-wrapper">
          <div class="ebook-loading-line ebook-loading-line-02"></div>
        </div>
        <div class="ebook-loading-line-wrapper">
          <div class="ebook-loading-line ebook-loading-line-03"></div>
        </div>
      </div>
      <div class="ebook-loading-item">
        <div class="ebook-loading-line-wrapper">
          <div class="ebook-loading-line ebook-loading-line-04"></div>
        </div>
        <div class="ebook-loading-line-wrapper">
          <div class="ebook-loading-line ebook-loading-line-05"></div>
        </div>
        <div class="ebook-loading-line-wrapper">
          <div class="ebook-loading-line ebook-loading-line-06"></div>
        </div>
      </div>
      <div class="ebook-loading-center"></div>
    </div>
  </div>
</template>

<script>
  export default {}
</script>

<style lang="scss" scoped>
  @import "../../assets/styles/global";
  .ebook-loading {
    position: relative;
    z-index: 500;
    width: px2rem(63);
    height: px2rem(40);
    background: transparent;
    border: px2rem(1.5) solid #d7d7d7;
    border-radius: px2rem(3);
    .ebook-loading-wrapper {
      display: flex;
      width: 100%;
      height: 100%;
      .ebook-loading-item {
        display: flex;
        flex-direction: column;
        flex: 1;
        padding: px2rem(7) 0;
        box-sizing: border-box;
        .ebook-loading-line-wrapper {
          flex: 1;
          padding: 0 px2rem(7);
          box-sizing: border-box;
          @include left;
          .ebook-loading-line {
            flex: 0 0 px2rem(16);
            width: px2rem(16);
            height: px2rem(1.5);
            background: #d7d7d7;
            animation: loading .7s infinite linear alternate;
            &.ebook-loading-line-01{
              animation-delay: 100ms;
            }
            &.ebook-loading-line-02{
              animation-delay: 250ms;
            }
            &.ebook-loading-line-03{
              animation-delay: 400ms;
            }
            &.ebook-loading-line-04{
              animation-delay: 550ms;
            }
            &.ebook-loading-line-05{
              animation-delay: 700ms;
            }
            &.ebook-loading-line-06{
              animation-delay: 850ms;
            }
          }
        }
      }
      .ebook-loading-center {
        position: absolute;
        left: 50%;
        top: 0;
        width: px2rem(1.5);
        height: 100%;
        background: #d7d7d7;
      }
    }
  }
</style>
