<template>
  <div class="root">
      <ShortCut class="w"></ShortCut>
      <indexHeader class="w"></indexHeader>
      <top class="w"></top>
  </div>
</template>

<script>
import ShortCut from "./ShortCut.vue"
import indexHeader from './indexHeader.vue'
import top from './top.vue'

export default {
    name: "Home",
    components: {
        ShortCut,
        indexHeader,
        top,
    }
}
</script>

<style>

 .w {
     width:1190px ;
     margin: 0 auto;
 }

 .root {
     background-color: var(--gray-bg);
 }
 li {
     list-style: none;
 }
</style>
