<template>
  <HelloWorld msg="Welcome App"/>
  <VFor> </Vfor>
  <For></For>
  <Aisatsu></Aisatsu>
  <Form></Form>
  <ColorChange></ColorChange>
  <LeftRight></LeftRight>
</template>

<script>
import HelloWorld from './components/HelloWorld.vue'
import VFor from './components/VFor'
import For from './components/For'
import Aisatsu from './components/Aisatsu'
import Form from './components/Form'
import ColorChange from './components/ColorChange'
import LeftRight from './components/LeftRight'


export default {
  name: 'App',
  components: {
    HelloWorld,
    VFor,
    For,
    Aisatsu,
    Form,
    ColorChange,
    LeftRight
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
