<template>
  <div class="middle-footer-components-container">
      <div class="info-links-container">
          <div class="section-link">
            <h4>dc comics</h4>
            <ul>
                <li v-for="(element, index) in comicslink" :key="index">{{element.text}}</li>
            </ul>              
          </div>

          <div class="section-link">
            <h4>shop</h4>
            <ul>
                <li v-for="(element, index) in shoplink" :key="index">{{element.text}}</li>
            </ul> 
          </div>

          <div class="section-link">
            <h4>dc</h4>
            <ul>
                <li v-for="(element, index) in dclink" :key="index">{{element.text}}</li>
            </ul>
          </div>

          <div class="section-link">
            <h4>sites</h4>
            <ul>
                <li v-for="(element, index) in siteslink" :key="index">{{element.text}}</li>
            </ul>              
          </div>

      </div>



      <div class="img-dc-container">
          <img src="../../../assets/img/dc-logo-bg.png" alt="">
      </div>
  </div>
</template>

<script>


export default {
  name: 'MiddleFooterComponents',
  data() {
      return{
          comicslink: [
                {
                    text:'Characters'
                },
                {
                    text:'Comics'
                },
                {
                    text:'Movies'
                },
                {
                    text:'TV'
                },
                {
                    text:'Games'
                },
                {
                    text:'Videos'
                },
                {
                    text:'News'
                }
          ],  
           shoplink: [
                {
                text:'Shop DC'
                },
                {
                text:'Shop DC Collectibles'
                }
          ],             
           dclink: [
                {
                    text:'Terms Of Use'
                },
                {
                    text:'Privacy policy (New)'
                },
                {
                    text:'Ad Choises'
                },
                {
                    text:'Advertising'
                },
                {
                    text:'Jobs'
                },
                {
                    text:'Subscriptions'
                },
                {
                    text:'Talent Workshops'
                },
                {
                    text:'CPSC Certificates'
                },
                {
                    text:'Ratings'
                },
                {
                    text:'Shop Help'
                },
                {
                    text:'Contact Us'
                }
          ],
           siteslink: [
                {
                    text:'DC'
                },
                {
                    text:'MAD Magazine'
                },
                {
                    text:'DC Kids'
                },
                {
                    text:'DC Universe'
                },
                {
                    text:'DC Power Visa'
                },
          ]         
      }
},

  components: {
  }
}

</script>

<style lang="scss" scoped>
    .middle-footer-components-container{
        display: flex;
        justify-content: space-between;
        align-items: center;
        width: 60%;
        height: 100%;

        .info-links-container{
            width: 40%;
            height: 200px;
            display: flex;
            justify-content: center;
            align-items: center;
            
            .section-link{
                height: 100%;
                color: rgb(255, 255, 255);
                text-transform: uppercase;
                margin: 10px;

                h4{
                    font-size: 12px;
                }


                
                li{
                    list-style: none;
                    color: rgba(117, 149, 117, 0.8);
                    font-size: 9px;
                    cursor: pointer;
                }
            }
        }

        .img-dc-container{
            width: 40%;
            height: 100px;
            display: flex;
            align-items: center;

            img{
                width: 100%;
                display: flex;
                justify-content: end;
                align-items: center;
            }
        }
    }
</style>