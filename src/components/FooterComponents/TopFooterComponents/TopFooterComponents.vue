<template>
  <div class="buy-comics-container">
    <div class="service-container" v-for="(element, index) in buydcproduct" :key="index">
      <img :src="element.img" alt="">
      <div>{{element.text}}</div>
    </div>
  </div>
</template>

<script>


export default {
  name: 'TopFooterComponents',
  data(){
    return{
      buydcproduct: [
        {
          img: require("../../../assets/img/buy-comics-digital-comics.png"),
          text: 'digital comics'
        },
        {
          img: require("../../../assets/img/buy-comics-merchandise.png"),
          text: 'dc merchandise'
        },
        {
          img: require("../../../assets/img/buy-comics-subscriptions.png"),
          text: 'subscription'
        },
        {
          img: require("../../../assets/img/buy-comics-shop-locator.png"),
          text: 'comic shop locator'
        },
        {
          img: require("../../../assets/img/buy-dc-power-visa.svg"),
          text: 'dc power visa'
        }                        
      ]
    }
  },
  components: {
  }
}
</script>

<style lang="scss" scoped>
    .buy-comics-container{
        width: 60%;
        color: rgb(255, 255, 255);
        text-transform: uppercase;
        font-size: 12px;
        display: flex;
        justify-content: space-around;
        align-items: center;
        text-align: center;

        img{
            height: 60px;
            margin-bottom: 10px;
        }
    }
</style>