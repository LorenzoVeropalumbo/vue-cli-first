<template>
  <div>
    <h1>{{ msg }}</h1>
  </div>
</template>

<script>
  export default {
    name: 'HeroComponent',
    props: {
      msg: String
    }, 
  }
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style>
  h1 {
   color: #2c3e50;
   font-size: 60px;
  }
</style>
