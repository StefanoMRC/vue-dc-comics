<template>
  <div>
      <ul>
          <li></li>
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
div{
    background: red;
    padding: 0;
    margin: 0;
    width: 40%;
    text-align: center;
}
</style>