<template>
  <div class="slideMin">
    <div class="slides" v-for="(pics, index) in slides" :key="index">
       <slide :height="height" :pics="pics" ip="none" :img="img" ></slide>
    </div>
  
  </div>
  
</template>

<script>

import slide from "./slide.vue"
export default {
  props: {
    slides:[],
    img: Boolean
  },
  data(){
    return{
      height:"153px"
    }
  },
  name: "slideMin",
  components:{
    slide
  }
  
};


</script>

<style>
.slides:nth-child(-n+2) {
  padding-bottom: 10px;
}



</style>