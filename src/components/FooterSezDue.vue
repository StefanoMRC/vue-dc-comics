<template>
  <div>
     <div class="cont">
         <div class="contLeft">
             <button type="button" class="bottone">sign-up now!</button>
         </div>
         <div class="contRight">
             <p>
                 <span class="contText">
                        follow us
                 </span>
                 <span class="contImg">
                        <img src="../assets/img/footer-facebook.png" alt="">
                        <img src="../assets/img/footer-twitter.png" alt="">
                        <img src="../assets/img/footer-youtube.png" alt="">
                        <img src="../assets/img/footer-pinterest.png" alt="">
                        <img src="../assets/img/footer-periscope.png" alt="">
                 </span>
             </p>
         </div>
     </div>
  </div>
</template>

<script>
export default {
  name: 'ComponentLogo',

}
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped lang="scss">
@import '../assets/style/variabili.scss';
@import '../assets/style/mixin.scss';
div{
    padding: 8px 0;
    background: #303030;
    .cont{
        width: 78%;
        margin: auto;
        display: flex;
        align-items: center;
        
        .contLeft{
            width: 50%;
            text-align: left;
            .bottone{
                background: #303030;
                color: $bianco;
                text-transform: uppercase;
                padding: 10px ;
                border: 1px solid $blu;
                font-size: 1.2em;
            }
            .bottone:hover{
                color: $blu;
            }
        }
        .contRight{
            width: 50%;
            
            p{
                display: flex;
                align-items: center;
                justify-content: end;
                .contText{
                    font-size: 1.5em;
                    text-transform: uppercase;
                    color: $blu;
                    margin-right: 10px;
                    font-weight: bold;
                }
                .contImg{
                    img{
                        margin: 0 5px;
                    }
                }
            }
        }
    }
}
</style>
