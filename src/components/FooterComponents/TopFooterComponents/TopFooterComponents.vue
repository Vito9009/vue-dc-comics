<template>
  <div class="buy-comics-container">
      <img src="../../../assets/img/buy-comics-digital-comics.png" alt="">
      <span>digital comics</span>
  </div>
</template>

<script>


export default {
  name: 'TopFooterComponents',
  components: {
  }
}
</script>

<style lang="scss" scoped>
    .buy-comics-container{
        width: calc(100% / 5);
        color: rgb(255, 255, 255);
        text-transform: uppercase;
        font-size: 15px;
        display: flex;
        justify-content: center;
        align-items: center;


        img{
            height: 60px;
            margin-right: 10px;
        }
    }
</style>