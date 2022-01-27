<template>
  <div class="my_middle-footer-container">
    <MiddleFooterComponents />
  </div>
</template>

<script>
import MiddleFooterComponents from './MiddleFooterComponents/MiddleFooterComponents.vue'


export default {
  name: 'MiddleFooter',
  components: {
    MiddleFooterComponents
  }
}
</script>

<style lang="scss" scoped>
@import '../../assets/my_scss/partials/variables.scss';

.my_middle-footer-container{
  height: 300px;
  width: 100%;
  background-image: url('../../assets/img/footer-bg.jpg');
  background-position: center;
  background-size: cover;
  background-repeat: no-repeat;
  display: flex;
  justify-content: center;
  overflow: hidden;
}

</style>