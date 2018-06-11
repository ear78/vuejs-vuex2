<template>
  <div>
    <h1>{{ title }}</h1>

    <ul class="navigation">
      <li>Test Li</li>
    </ul>
  </div>
</template>

<script>
    export default {
        name: 'Home',
        data(){
          return {
            title: 'This is the home page...'
          }
        }
    }
</script>

<style scoped>

</style>
