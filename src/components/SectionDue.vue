<template>
  <div>
      <ul>
          <li v-for="(element, index) in listaSez2" :key="index">
              <img :src="`${element.img}`" alt="">
              <h2>{{element.nome}}</h2>
          </li>
      </ul>
  </div>
</template>

<script>
import image from "../assets/img/buy-comics-digital-comics.png"
import image1 from "../assets/img/buy-comics-merchandise.png"
import image2 from "../assets/img/buy-comics-subscriptions.png"
import image3 from "../assets/img/buy-comics-shop-locator.png"
import image4 from "../assets/img/buy-dc-power-visa.svg"

export default {

  name: 'SectionDue',
  data() {
      return {
          listaSez2:[
                {
                  img:image,
                  nome:'digital comics'
                },
                 {
                   img:image1,
                   nome:'dc merchandise'
                 },
                 {
                   img:image2,
                   nome:'subscriptions'
                 },
                 {
                   img:image3,
                   nome:'comic shop locator'
                 },
                 {
                   img:image4,
                   nome:'dc power visa'
                 },
          ]
      }
  },

}
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped lang="scss">
@import '../assets/style/mixin.scss';
@import '../assets/style/variabili.scss';
div{
    background: $blu;
    text-align: center;

   ul{
      width: 80%;
       @include lista(space-between, row, center);
            margin: auto;
            padding: 0;
        li{
            display: flex;
            align-items: center;
            padding: 20px;
            text-transform: uppercase;
            color: $bianco;
            font-size: 0.5em;
            img{
                max-width: 60px;
                height: 50px;
                padding: 0 10px;
            }
        }    
   }
}
</style>