<template>
  <div id="app">
    <One></One>
    <Two></Two>
    <Three></Three>
    <Four></Four>
    <Five></Five>
  </div>
</template>

<script>
import One from '@/components/One'
import Two from '@/components/Two'
import Three from '@/components/Three'
import Four from '@/components/Four'
import Five from '@/components/Five'
export default {
  name: 'App',
  components:{One,Two,Three,Four,Five}
}
</script>

<style>
#app {
  font-family: 'Avenir', Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  text-align: center;
  color: #2c3e50;
  margin-top: 60px;
}
</style>
