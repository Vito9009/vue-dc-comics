<template>
  <div class="my_main-container">
    <div class="jumbo">

    </div>
    <div class="main-showcase">
      <div class="showcase-content">
        <MultiThumb />
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
    .my_main-container{
        width: 100%;
        background-color: rgb(28, 28, 28);


        .main-showcase{
          color: rgb(255, 255, 255);
          display: flex;
          justify-content: center;
          align-items: center;

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
    }
</style>