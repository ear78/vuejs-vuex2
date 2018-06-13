<template>
  <div id="app">
    <Header></Header>
    <router-view/>
  </div>
</template>

<script>
  import Header from './components/ui-components/Header'
export default {
  name: 'App',
  components: {
    Header: Header
  }
}
</script>

<style>
  @import '../node_modules/reset-css/reset.css';

#app {
  font-family: 'Avenir', Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  text-align: center;
  color: #2c3e50;
  margin-top: 60px;
}
  h1 {
    font-size: 2em;
    font-weight: 600;
  }

  ul {
    list-style-type: none;
  }

  a {
    color: #2c3e50;
    text-decoration: none;
  }

  .max-text-width {
    margin: 0 auto;
    max-width: 800px;
    padding: 0 15px;
  }

  .margin-bottom-md {
    margin-bottom: 30px;
  }
</style>
