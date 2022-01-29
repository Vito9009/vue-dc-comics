<template>
<div>
  <div class="my_main-container">
    <div class="jumbo">

    </div>

     <button class="top-btn">current series</button>

    <div class="main-showcase">
      <div class="showcase-content">
        <MultiThumb />
      </div>
    </div>
    <div class="bottom-btn-container">
       <button class="bottom-btn">load more</button>
    </div>
  </div>
</div>

</template>

<script>
import MultiThumb from './MainComponents/MultiThumb.vue'

export default {
  name: 'Main',
  components: {
    MultiThumb
  }
}
</script>

<style lang="scss" scoped>
@import '../assets/my_scss/partials/variables.scss';

    .my_main-container{
        width: 100%;
        background-color: rgb(28, 28, 28);


        .main-showcase{
          color: rgb(255, 255, 255);
          display: flex;
          justify-content: center;
          align-items: center;
          padding: 20px 0;

          .showcase-content{
            width: 65%;
          }
        }

        .jumbo{
          background-image: url("../assets/img/jumbotron.jpg");
          background-size: cover;
          height: 600px;
          width: 100%;
        }

        .top-btn{
          position: absolute;
          left: 15%;
          top: 730px;
          padding: 10px 15px;
        }
    }

    .bottom-btn-container{
      width: 100%;
      height: 50px;
      display: flex;
      justify-content: center;
      align-items: center;

      .bottom-btn{
        margin-bottom: 50px;
        padding: 10px 30px;
      }
    }

    .bottom-btn, .top-btn{
      background-color: $blueComics;
      color: rgb(255, 255, 255);
      text-transform: uppercase;
      font-weight: bold;
      border: 0;
    }
</style>