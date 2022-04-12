<template>
  <div>
      <ul>
          <li v-for="(element, index) in listaSez2" :key="index">
              <img :src="`../assets/img/${element.img}`" alt="">
              <h2>{{element.nome}}</h2>
          </li>
      </ul>
  </div>
</template>

<script>
export default {
  name: 'SectionDue',
  data() {
      return {
          listaSez2:[
                {
                  img:'buy-comics-digital-comics.png',
                  nome:'digital comics'
                },
                {
                  img:'buy-comics-merchandise.png',
                  nome:'dc merchandise'
                },
                {
                  img:'buy-comics-subscriptions.png',
                  nome:'subscriptions'
                },
                {
                  img:'buy-comics-shop-locator.png',
                  nome:'comic shop locator'
                },
                {
                  img:'buy-dc-power-visa.svg',
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
       @include lista(center, row, center);
            margin: 0;
            padding: 0;
        li{
            display: flex;
            padding: 20px;
            text-transform: uppercase;
            color: $bianco;
            font-size: 0.5em;
        }    
   }
}
</style>