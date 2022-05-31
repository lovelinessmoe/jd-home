<template>
  <el-carousel  :height="height" :indicator-position="ip" :arrow="arrow" :interval='interval'>
    <el-carousel-item v-for="(pic, index) in pics" :key="index">
       <img :src="pic.url" alt="" v-if="img">
      <a href=""><span v-if="!img">{{pic.url}}</span></a>
    </el-carousel-item>
  </el-carousel>
</template>

<script>

export default {
  
  name: "slide",
  data(){
  console.log(this.narrow);
    return {
      
    }
},
  props: ['pics','height','ip','img','arrow','interval']
  
};


</script>

<style>
.el-carousel__item img {
  width: 100%;
  height: 100%;
}



</style>