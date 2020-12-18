/* eslint-disable */
<template>
  <!-- 案例4-->
  <div class="example">
    <div>{{ num }}
    <button @click="check" >check</button>
    </div>
  </div>
</template>
<script setup>
  import {ref} from "vue"; //可以不用声明
  ref:num=100
  ref:color1='red'
  ref:color2='green'
  const colorArr=['red','green','aquamarine','aquam']
  function check(){
    const index = Math.floor(Math.random() * colorArr.length)
    const index2 = Math.floor(Math.random() * colorArr.length)
    color1=colorArr[index]
    color2=colorArr[index2]
  }
</script>
/* eslint-disable */
<style scoped lang="scss">
.example {
  display: flex;
  height: 150px;
  width: 150px;
  justify-content: center;
  align-items: center;
  color: v-bind(color1);
  background-color:v-bind(color2);
}
</style>


