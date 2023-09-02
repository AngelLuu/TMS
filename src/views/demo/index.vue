<!--  -->
<template>
  <div class='container'>
    <div class="top">

    </div>
    <div class="cen"></div>
    <div class="bom"></div>
  </div>
</template>

<script setup lang='ts'>
import { reactive } from 'vue'
// import {} from ''

const str = reactive({
  name: '测试页面'
})
</script>

<style scoped>
.container {
  width: 100%;
  padding: 4px;
  display: flex;
  flex: 1;

  .top {
    /* display: flex; */
    width: 100%;
  }
}</style>