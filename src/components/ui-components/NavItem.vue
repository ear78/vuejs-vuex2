<template>
  <router-link v-bind:to="links" tag="li" active-class="active"><a>{{ links.link }}</a></router-link>
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

</style>
