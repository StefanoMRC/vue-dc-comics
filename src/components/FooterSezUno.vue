<template>
  <div class="cont">
      <div>
          <div>
                <h2>dc comics</h2>

                <ul>             
                    <li v-for="(element,index) in comicsList" :key="index">
                        <a :href="`${element.link}`">{{element.nome}}</a>
                    </li>
                </ul>

                <h2>shop</h2>

                <ul>
                    <li v-for="(element,index) in shopList" :key="index">
                        <a :href="`${element.link}`">{{element.nome}}</a>
                    </li>
                </ul>
          </div>

        </div>
      <div>
          <h2>dc</h2>

          <ul>
              <li v-for="(element,index) in dcList" :key="index">
                  <a :href="`${element.link}`">{{element.nome}}</a>
              </li>
          </ul>
      </div>
      <div>
          <h2>sites</h2>
          <ul>
              <li v-for="(element,index) in sitesList" :key="index">
                  <a :href="`${element.link}`">{{element.nome}}</a>
              </li>
          </ul>
      </div>
  </div>
</template>

<script>
export default {
  name: 'FooterSezUno',
    data() {
        return {
            comicsList:[
                {
                    nome:'Characters',
                    link:'characters/'
                },
                {
                    nome:'Comics',
                    link:'comics/'
                },
                {
                    nome:'Movies',
                    link:'movies/'
                },
                {
                    nome:'TV',
                    link:'tv/'
                },
                {
                    nome:'Games',
                    link:'games/'
                },
                {
                    nome:'Videos',
                    link:'videos/'
                },
                {
                    nome:'News',
                    link:'news/'
                },    
            ],
            shopList:[
                {
                    nome:'Shop DC',
                    link:'shop-dc/'
                },
                {
                    nome:'Shop DC Collectibles',
                    link:'shop-dc-collectibles/'
                }
            ],
            dcList:[
                {
                    nome:'Terms Of Use',
                    link:'terms-of-use/'
                },
                {
                    nome:'Private policy(New)',
                    link:'private-policy/'
                },
                {
                    nome:'Ad Choices',
                    link:'ad-choices/'
                },
                {
                    nome:'Advertising',
                    link:'advertising/'
                },
                {
                    nome:'Jobs',
                    link:'jobs/'
                },
                {
                    nome:'Subscription',
                    link:'subscription/'
                },
                {
                    nome:'Talent Workshops',
                    link:'talent-workshops/'
                },
                {
                    nome:'CPSC Certificates',
                    link:'cpsc-certificates/'
                },
                {
                    nome:'Ratings',
                    link:'ratings/'
                },
                {
                    nome:'Shop Help',
                    link:'shop-help/'
                },
                {
                    nome:'Contact Us',
                    link:'contact-us/'
                },
            ],
            sitesList:[
                {
                    nome:'DC',
                    link:'dc/'
                },
                {
                    nome:'MAD Magazine',
                    link:'mad-magazine/'
                },
                {
                    nome:'DC Kids',
                    link:'dc-kids/'
                },
                {
                    nome:'DC Universe',
                    link:'dc-universe'
                },
                {
                    nome:'DC Power Visa',
                    link:'dc-power-visa'
                },
            ]
        }
    },
}
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped lang="scss">
@import '../assets/style/variabili.scss';
@import '../assets/style/mixin.scss';
.cont{
    display: flex;
    background-image: url(../assets/img/footer-bg.jpg);
}
   
    h2{
        color: $bianco;
        text-transform: uppercase;
        font-size: 1em;  
    }
    ul{
    @include lista(center, column, center);
            margin: 0;
            padding: 0 30px;
        li{
            a{
                padding: 10px 0;
                text-decoration: none;
                color: $grigio;
            }
        }
    }


</style>
