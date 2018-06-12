<template>
  <router-link v-bind:to="links" tag="li" active-class="active" class="nav-link"><a>{{ links.link }}</a></router-link>
</template>

<script>
  export default {
    props: ['links'],
    name: 'nav-item',
    data(){
      return {

      }
    }
  }


</script>

<style scoped>
  .nav-link {
    margin: 0 5px;
  }

  .nav-link:hover a {
    color: gray;
  }
</style>
