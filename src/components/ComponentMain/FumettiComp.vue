<template>
  
      
      
         
            <div>
              <div class="contImg"></div> 
              <img :src="img" alt="">
              <h3>{{titolo}}</h3>
            </div>
          
       


    
  
</template>

<script>
export default {
  name: 'FumettiComp',
    props:{
        img:String,
        titolo:String
    }
}
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped lang="scss">
                div{
                    margin: 5px 30px;
                    flex-basis: calc((100%/6) - 60px);
                    img{
                        width: 100%;
                    }
                    h3{
                        color: white;
                    }
                }

        
    
</style>
