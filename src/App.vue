<template>
  <div id="app">
    <HeaderDc/>
    <Content/>
    <Merchandise/>
    <Jumbo/>
  </div>
</template>

<script>
import HeaderDc from './components/HeaderDc.vue';
import Content from './components/Content.vue';
import Merchandise from './components/Merchandise.vue';
import Jumbo from './components/Jumbo.vue';

export default {
  name: 'App',
  components: {
    HeaderDc,
    Content,
    Merchandise,
    Jumbo
  }
}
</script>

<style lang="scss">
#app {
  font-family: Avenir, Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
}

*{
  margin: 0;
  padding: 0;
  box-sizing: border-box;
}
</style>
