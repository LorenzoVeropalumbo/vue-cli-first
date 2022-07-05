<template>
  <div>
    <img :src="imageChanger[index].url" @click="bigImg">
  </div>
</template>

<script>
  export default {
    name: 'TitleComponent',
    data(){
      return{  
        index: 0,
        imageChanger:[
          {
            url:require("../assets/01.jpg")
          },
          {
            url:require("../assets/02.jpg")
          },
          {
            url:require("../assets/03.jpg")
          },
          {
            url:require("../assets/04.jpg")
          },
          {
            url:require("../assets/05.jpg")
          },
        ]
      }
    },
    methods:{
      bigImg(){
        if(this.index >= this.imageChanger.length - 1){
          this.index = 0;
        } else {
          this.index++;
        }
        
      }      
    }
  }
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style>
  img{
    width: 550px;
    border: 2px solid red;
    height: 400px;
  }
</style>
