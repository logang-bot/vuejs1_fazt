<template>
  <div id="app"> 
    <h1>hola mundo</h1>
    <test msg="hola!!!!!!"/>
    <user/>
  </div>
</template>

<script>

import test from './components/test.vue'
import User from './components/user.vue'
import user from './components/user.vue'

export default {
  name: 'App',
  components: {
    test,
    User
  }
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
