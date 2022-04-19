<template>
  <div>
      <ul>
          <li v-for="(element, id) in menuTop" :key="id">
              <a href="`${element.link}`">{{element.nome}}</a>
          </li>
      </ul>
  </div>
</template>

<script>
export default {
  name: 'MenuHeaderComp',
    data() {
        return {
            menuTop:[
                {
                    nome:'characters',
                    link:'/characters'
                },
                                {
                    nome:'comics',
                    link:'/comics'
                },
                                {
                    nome:'movies',
                    link:'/movies'
                },
                                {
                    nome:'tv',
                    link:'/tv'
                },
                                {
                    nome:'games',
                    link:'/games'
                },
                                {
                    nome:'collectibles',
                    link:'/collectibles'
                },
                                {
                    nome:'videos',
                    link:'/videos'
                },
                                {
                    nome:'fans',
                    link:'/fans'
                },
                                {
                    nome:'news',
                    link:'/news'
                },
                                {
                    nome:'shop',
                    link:'/shop'
                }

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
     width: 80%;
     margin: 0 auto;
         ul{
            @include lista(end, row, center);
            margin: 0;
            padding: 0;
            height: 98%;
                li{
                    height: 100%;
                    padding:0 10px;
                    font-size: 1.2em;
                    text-transform: uppercase;
                    display: flex;
                    align-items: center;
                    &:hover{
                        border-bottom: 3px solid $blu;
                        a{
                            color: $blu;
                        }
                    }
                        a{
                            text-decoration: none;
                            padding: 50px 0;
                            color: $nero;
                            font-weight: bold;
                        }
                }

        }
    }   


</style>