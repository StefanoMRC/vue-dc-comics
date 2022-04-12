<template>
    <header>
      <ComponentLogo/>
    </header>
</template>

<script>
// import HelloWorld from './components/HelloWorld.vue'
import ComponentLogo from './components/ComponentLogo.vue'

export default {
  name: 'App',
  components: {
    // HelloWorld
    ComponentLogo
  }
}
</script>

<style lang="scss">
  body{
    margin: 0;
  }
</style>
