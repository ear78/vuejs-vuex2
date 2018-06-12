
<template>
  <div>
    <h1 class="margin-bottom-md">{{ title }}</h1>
    <p class="max-text-width">Lorem Ipsum is simply dummy text of the printing and typesetting industry. Lorem Ipsum has been the industry's standard dummy text ever since the 1500s, when an unknown printer took a galley of type and scrambled it to make a type specimen book.</p>
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
