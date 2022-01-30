<template>
  <div class="bottom-footer-content-container">
    <div class="btn-footer-container">
      <button class="footer-btn">sign-up now!</button>
    </div>

    <div class="social-container">
      <div class="follow-text">follow us</div>
      <div class="social-icons-container" v-for="(element, index) in socialicons" :key="index">
        <img :src="element.icon" alt="">
      </div>
    </div>
  </div>
</template>

<script>
export default {
    name: 'BottomFooterComponents',
    data() {
      return{
        socialicons: [
          {
            icon: require("../../../assets/img/footer-facebook.png")
          },
          {
            icon: require("../../../assets/img/footer-twitter.png")
          },
          {
            icon: require("../../../assets/img/footer-youtube.png")
          },
          {
            icon: require("../../../assets/img/footer-pinterest.png")
          },
          {
            icon: require("../../../assets/img/footer-periscope.png")
          }
        ]
      }
    }
}
</script>

<style lang="scss" scoped>
@import '../../../assets/my_scss/partials/variables.scss';

.bottom-footer-content-container{
  height: 100%;
  display: flex;

    .btn-footer-container, .social-container {
      width: 50%;
      height: 100%;
      display: flex;
      justify-content: center;
      align-items: center;

      .footer-btn{
        border: 2px solid $blueComics;
        background-color: rgba(0, 0, 0, 0);
        color: rgb(255, 255, 255);
        text-transform: uppercase;
        font-weight: bold;
        padding: 10px;
        cursor: pointer;
      }
    }

    .social-container {
      color: $blueComics;
      text-transform: uppercase;
      font-weight: bold;

      .follow-text{
        margin-right: 30px;
      }


      .social-icons-container{
        width: 50px;
        display: flex;
        justify-content: space-around;

        img{
          width: 30px;
          cursor: pointer;
        }
      }
    }
}


</style>