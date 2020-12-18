<template>
  <!-- 案例4-->
  <div class="example">
    <div>{{ num }}
    <button @click="check" >check</button>
    </div>
  </div>
</template>
<script setup>
  import {ref} from "vue";
  ref:num=100
  function check(){
    num=1
  }
</script>

<style scoped lang="scss">
.example {
  display: flex;
  height: 50px;
  width: 50px;
  justify-content: center;
  align-items: center;
  color: red;
  background-color: black;
}
</style>


