<template>
  <!-- dynamically building menu using single li component passing props from parent to child -->
  <ul class="navigation">
    <NavItem v-bind:links="i" v-for="i in menu"></NavItem>
  </ul>
</template>

<script>
  import NavItem from './NavItem';

  export default {
    name: 'Header',
    components: {
      NavItem: NavItem
    },
    data(){
      return {
        title: 'This is the home page...',
        menu: [
          {
            path: '/',
            link: 'Home'
          },
          {
            path: '/about',
            link: 'About'
          },
          {
            path: '/contact',
            link: 'Contact'
          }
        ]
      }
    }
  }
</script>

<style>

  .active {
    color: blue;
  }
</style>
