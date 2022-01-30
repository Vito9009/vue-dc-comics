<template>
  <div class="my_bottomfooter-container">
      <BottomFooterComponents />
  </div>

</template>

<script>
import BottomFooterComponents from './BottomFooterComponents/BottomFooterComponents.vue'


export default {
  name: 'BottomFooter',
  components: {
    BottomFooterComponents
  }
}
</script>

<style lang="scss" scoped>
@import '../../assets/my_scss/partials/variables.scss';

.my_bottomfooter-container{
  height: 100px;
  width: 100%;
  background-color: rgb(48, 48, 48);
}
</style>