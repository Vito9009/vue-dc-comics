<template>
  <header>
      <a href="#" class="navbar-icon">
          <img src="../assets/img/dc-logo.png" alt="">
      </a>

      <ul class="my_navbar-container">
          <li v-for="(element, index) in links" :key="index">
              <a href="#" :class="{'active': element.current}">{{element.text}}</a>
          </li>

      </ul>
  </header>
</template>

<script>


export default {
  name: 'Header',
      data() {
      return{
        links: [
            {
                text: "Characters",
                url: "#",
                current: false,
            },
            {
                text: "Comics",
                url: "#",
                current: true,
            },
            {
                text: "Movies",
                url: "#",
                current: false,
            },
            {
                text: "TV",
                url: "#",
                current: false,
            },
            {
                text: "Games",
                url: "#",
                current: false,
            },
            {
                text: "Collectibles",
                url: "#",
                current: false,
            },
            {
                text: "Videos",
                url: "#",
                current: false,
            },
            {
                text: "Fans",
                url: "#",
                current: false,
            },
            {
                text: "News",
                url: "#",
                current: false,
            },
            {
                text: "Shop",
                url: "#",
                current: false,
            },
        ]
      }
    },
  components: {
  }
}
</script>

<style lang="scss" scoped>
@import '../assets/my_scss/partials/variables.scss';

    header{
        height: 150px;
        display: flex;
        justify-content: space-around;
        background-color: rgb(255, 255, 255);

        .navbar-icon{
            width: 20%;
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
            align-items: flex-end;
            margin: 0;

            li{
                height: 100%;
                display: flex;
                justify-content: center;
                align-items: flex-end;
                padding: 0 20px;
                text-transform: uppercase;
                font-size: 12px;

                a{
                    text-decoration: none;
                    height: 150px;
                    color: rgb(0, 0, 0);
                    line-height: 150px;

                    &.active, &:hover{
                        border-bottom: 3px solid $blueComics;
                        color: $blueComics;
                    }
                }
                
            }
        }
    }
</style>