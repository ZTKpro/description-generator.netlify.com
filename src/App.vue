<template>
<main>
  <div id="app">
    <Generator />
  </div>
  </main>
</template>

<script>
import Generator from './components/Generator.vue'

export default {
  name: 'app',
  components: {
    Generator
  }
}
</script>

<style>
#app {
  font-family: 'Avenir', Helvetica, Arial, sans-serif;
  text-align: center;
  color: #2c3e50;
  margin-top: 30px;
}
</style>
