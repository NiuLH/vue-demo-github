<template>
  <HelloWorld/>
  <SlotParent/>
</template>

<script>
import HelloWorld from './components/HelloWorld.vue'
import SlotParent from './components/SlotParent.vue'

export default {
  name: 'App',
  components: {
    HelloWorld,
    SlotParent
  }
}
</script>

<style>
#app {
  font-family: Avenir, Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  text-align: center;
  color: #2c3e50;
  margin-top: 60px;
}
</style>
