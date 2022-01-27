<template>
  <header>
      <a href="#" class="navbar-icon">
          <img src="../assets/img/dc-logo.png" alt="">
      </a>

      <ul class="my_navbar-container">
          <li>Characters</li>
          <li>Comics</li>
          <li>Movies</li>
          <li>TV</li>
          <li>Games</li>
          <li>Collectibles</li>
          <li>Videos</li>
          <li>Fans</li>
          <li>News</li>
          <li>Shop</li>
      </ul>
  </header>
</template>

<script>


export default {
  name: 'Header',
  components: {
  }
}
</script>

<style lang="scss" scoped>
    header{
        widows: 100%;
        height: 150px;
        display: flex;
        background-color: rgb(255, 255, 255);

        .navbar-icon{
            width: 35%;
            height: 100%;
            display: flex;
            justify-content: center;
            align-items: center;

            img{
                width: 100px;
            }
        }

        .my_navbar-container{
            list-style: none;
            display: flex;
            justify-content: space-around;
            align-items: center;
            margin: 0;

            li{
                height: 100%;
                display: flex;
                justify-content: center;
                align-items: center;
                padding: 0 20px;
                text-transform: uppercase;
            }
        }
    }
</style>