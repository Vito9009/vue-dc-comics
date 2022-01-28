<template>
  <div class="my_thumb">
      <img :src="multiinfo.thumb" :alt="multiinfo.series">
      <h4>{{multiinfo.series}}</h4>
  </div>
</template>

<script>
export default {
    name: 'SingleThumb',
    props: {
        'multiinfo': Object
    }
}
</script>

<style lang="scss" scoped>
    .my_thumb{
        width: calc((100% / 6) - 10px);
        margin: 20px 5px;
        text-align: center;
        

        img{
            width: 100%;
            height: 100%;
        }

        h4{
            text-transform: uppercase;
            font-size: 10px;
        }
    }
</style>