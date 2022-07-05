<template>
  <div>
    <img :src="imgPath" @click="bigImg">
  </div>
</template>

<script>
  export default {
    name: 'HelloWorld',
    data(){
      return{
        imgPath: "https://cdn.pixabay.com/photo/2015/04/23/22/00/tree-736885__480.jpg",
      }
    },
    methods:{
      bigImg(){
        console.log("adwadaw");
      }      
    }
  }
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style>
  img{
    width: 400px;
    border: 2px solid red;
    height: 300px;
  }
</style>
