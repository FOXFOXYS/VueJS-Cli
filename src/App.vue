<template>
  <div id="app">
    <Fuck/>
    <Button/>
    <Button/>
  </div>
</template>

<script>

import Button from './components/Button';
import Fuck from './components/Text';

export default {
  name: 'App',
  components: {
    Button,
    Fuck
  }
}
</script>

<style lang="scss">
#app {
  font-family: Avenir, Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  text-align: center;
  color: #2c3e50;
  margin-top: 60px;
}
</style>
