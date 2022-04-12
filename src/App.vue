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

    </div>
</template>

<script>
// import HelloWorld from './components/HelloWorld.vue'
import ComponentLogo from './components/ComponentLogo.vue'
import MenuHeaderComp from './components/MenuHeaderComp.vue'
import SectionUno from './components/SectionUno.vue'
import SectionDue from './components/SectionDue.vue'

export default {
  name: 'App',
  components: {
    // HelloWorld
    ComponentLogo,
    MenuHeaderComp,
    SectionUno,
    SectionDue
  }
}
</script>

<style lang="scss">
  body{
    margin: 0;
  }
  header{
    display: flex;

  }
</style>
