<template>
  <div>
     <h2>
          Content goes here 
     </h2>
  </div>
</template>

<script>
export default {
  name: 'SectionUno',

}
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped lang="scss">
@import '../assets/style/variabili.scss';
div{
    background: $nero;
    text-align: center;
    h2{
        font-size: 3em;
        color: $bianco;
        margin: 0;
        padding: 100px;
    }
}
</style>
