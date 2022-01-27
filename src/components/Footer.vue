<template>
  <div>
    <TopFooter />
    <MiddleFooter />
    <BottomFooter />

  </div>
</template>

<script>
import TopFooter from './FooterComponents/TopFooter.vue'
import MiddleFooter from './FooterComponents/MiddleFooter.vue'
import BottomFooter from './FooterComponents/BottomFooter.vue'

export default {
  name: 'Footer',
  components: {
      TopFooter,
      MiddleFooter,
      BottomFooter
  }
}
</script>

<style lang="scss" scoped>

</style>