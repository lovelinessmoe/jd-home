<template>
  <div class="hotwords">
    <ul>
      <li v-for="(word, index) in items" :key="index" style="color : colors"><a href="">{{ word.name }}</a> </li>
    </ul>
  </div>
</template>

<script>
export default {
  name: "NavItem",
  data() {
    return {
      color: "color",
      font_size: "font-size"
    }
  },
  props: ["items",'colors','fs'],
};
</script>

<style lang="less" scoped>
.hotwords {
 
  ul {
    
    li {
     
      display: inline-block;
      padding-right: 10px;
      &:hover{
          color: red;
      }
    }

  }
}
</style>