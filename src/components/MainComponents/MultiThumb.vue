<template>
  <div class="preview-container">
      <SingleThumb
        v-for="(img, index) in dcinfo"
        :key="index"
        :multiinfo="img"
       />
  </div>
</template>

<script>
import SingleThumb from './SingleThumb.vue'
import infohero from '../../JsData/Dc.js'

export default {
    name: 'MultiThumb',
    components: {
        SingleThumb
    },
    data(){
        return{
            dcinfo: infohero
            }
    }
}
</script>

<style lang="scss" scoped>
    .preview-container{
        display: flex;
        justify-content: space-between;
        flex-wrap: wrap;
        margin: 5px;  
    }
</style>