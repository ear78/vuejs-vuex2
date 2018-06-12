<template>
  <!-- dynamically building menu using single li component passing props from parent to child -->
  <ul class="navigation-container">
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
            path: 'info',
            link: 'Info'
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
  .router-link-active.active a,
  .router-link-exact-active.active a {
    color: lightgreen;
  }

  .navigation-container {
    display: flex;
    justify-content: center;
    padding: 20px 0 50px;
  }
</style>
