<template>
  <header>
      <a href="#" class="navbar-icon">
          <img src="../assets/img/dc-logo.png" alt="">
      </a>

      <ul class="my_navbar-container">
          <li><a href="">Characters</a></li>
          <li><a href="">Comics</a></li>
          <li><a href="">Movies</a></li>
          <li><a href="">TV</a></li>
          <li><a href="">Games</a></li>
          <li><a href="">Collectibles</a></li>
          <li><a href="">Videos</a></li>
          <li><a href="">Fans</a></li>
          <li><a href="">News</a></li>
          <li><a href="">Shop</a></li>
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
@import '../assets/my_scss/partials/variables.scss';

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

                a{
                    text-decoration: none;
                }
                
            }
        }
    }
</style>