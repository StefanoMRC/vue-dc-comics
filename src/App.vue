<template>
    <div>
      <header>
        <ComponentLogo/>
        <MenuHeaderComp/>
      </header>
      <main>
        <SectionUno/>
        <SectionDue/>
      </main>
      <footer>
        <FooterSezUno/>
        <FooterSezDue/>
      </footer>

    </div>
</template>

<script>
// import HelloWorld from './components/HelloWorld.vue'
import ComponentLogo from './components/ComponentLogo.vue'
import MenuHeaderComp from './components/MenuHeaderComp.vue'
import SectionUno from './components/SectionUno.vue'
import SectionDue from './components/SectionDue.vue'
import FooterSezUno from './components/FooterSezUno.vue'
import FooterSezDue from './components/FooterSezDue.vue'

export default {
  name: 'App',
  components: {
    // HelloWorld
    ComponentLogo,
    MenuHeaderComp,
    SectionUno,
    SectionDue,
    FooterSezUno,
    FooterSezDue
  }
}
</script>

<style lang="scss">
  @import url('https://fonts.googleapis.com/css2?family=Lato:ital,wght@1,300&family=Roboto:wght@300&display=swap');
  html{
    font-family: 'Roboto';
  }
  body{
    margin: 0;
    
  }
  header{
    display: flex;
    width: 80%;
    margin: 0 auto;
  }
</style>
