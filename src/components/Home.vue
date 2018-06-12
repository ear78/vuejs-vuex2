
<template>
  <div>
    <h1>{{ title }}</h1>

    <!-- dynamically building menu using single li component passing props from parent to child -->
    <ul class="navigation">
      <NavItem v-bind:links="i" v-for="i in menu"></NavItem>
    </ul>
  </div>
</template>

<script>
  import NavItem from './ui-components/NavItem';

    export default {
        name: 'Home',
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

<style scoped>

</style>
