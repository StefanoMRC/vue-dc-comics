<template>
  <div>
      <div class="hero">
        <button>
          current series
        </button>
      </div>
  </div>
</template>

<script>
export default {
  name: 'HeroComp',

}
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped lang="scss">
@import '../../assets/style/variabili.scss';
.hero{
    background-image: url("../../assets/img/jumbotron.jpg");
    height: 400px;
    background-size: cover;
    background-repeat: no-repeat;
    position: relative;
   button{
      font-size: 1.2em;
      text-transform: uppercase;
      padding: 5px 10px;
      background: $blu;
      color: $bianco;
      border: 0;
      position: absolute;
      bottom: -20px;
      left: 11%;
   }
}
</style>
