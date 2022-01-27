<template>
  <div class="my_top-footer-container">
      <div class="sub-top-footer-container">
        <TopFooterComponents />
        <TopFooterComponents />
        <TopFooterComponents />
        <TopFooterComponents />
        <TopFooterComponents />
      </div>
  </div>
</template>

<script>
import TopFooterComponents from './TopFooterComponents/TopFooterComponents.vue'

export default {
  name: 'TopFooter',
  components: {
      TopFooterComponents
  }
}
</script>

<style lang="scss" scoped>
@import '../../assets/my_scss/partials/variables.scss';

    .my_top-footer-container{
        background-color: $blueComics;
        height: 150px;
        width: 100%;
        display: flex;
        justify-content: center;
        align-items: center;


        .sub-top-footer-container{
            width: 60%;
            display: flex;
            justify-content: center;
            align-items: center;

        }
    }
</style>