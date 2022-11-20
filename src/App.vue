<template>
  <div id="app">
    <SimpleSlot />
    <DefaultContent />
    <NamedSlot />
    <ScopedSlot />
  </div>
</template>

<script>
import DefaultContent from './components/DefaultContent.vue';
import NamedSlot from './components/NamedSlot.vue';
import ScopedSlot from './components/ScopedSlot.vue';
import SimpleSlot from './components/SimpleSlot.vue';


export default {
  name: 'App',
  components: {
    SimpleSlot,
    DefaultContent,
    NamedSlot,
    ScopedSlot
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
  margin-top: 120px;
}
body {
  margin: 0;
}
</style>
