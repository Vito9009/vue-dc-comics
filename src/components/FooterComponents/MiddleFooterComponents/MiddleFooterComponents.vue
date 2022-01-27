<template>
  <div class="middle-footer-components-container">
      <div class="info-links-container">
          <h3>dasdas</h3>
          <div>dasdas</div>
          <div>dasdas</div>
          <div>dasdas</div>

      </div>

      <div class="img-dc-container">
          <img src="../../../assets/img/dc-logo-bg.png" alt="">
      </div>
  </div>
</template>

<script>


export default {
  name: 'MiddleFooterComponents',
  components: {
  }
}
</script>

<style lang="scss" scoped>
    .middle-footer-components-container{
        display: flex;
        justify-content: space-between;
        align-items: center;
        width: 60%;
        height: 100%;

        .info-links-container{
            width: 40%;
            height: 100%;
        }

        .img-dc-container{
            width: 40%;
            height: 100%;
            display: flex;
            align-items: center;

            img{
                width: 100%;
                display: flex;
                justify-content: end;
                align-items: center;
            }
        }
    }
</style>