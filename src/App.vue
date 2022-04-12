<template>
    <header>
      <ComponentLogo/>
      <MenuHeaderComp/>
    </header>
</template>

<script>
// import HelloWorld from './components/HelloWorld.vue'
import ComponentLogo from './components/ComponentLogo.vue'
import MenuHeaderComp from './components/MenuHeaderComp.vue'

export default {
  name: 'App',
  components: {
    // HelloWorld
    ComponentLogo,
    MenuHeaderComp
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
