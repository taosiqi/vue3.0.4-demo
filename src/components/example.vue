<template>
  <!-- 案例1-->
  <div class="example">
    <button @click="reduce">-</button>
    <div>{{num}}</div>
    <button @click="add">+</button>
  </div>
</template>

<script setup>
    import { ref } from "vue";
    let num=ref(0)
    // 这里onMounted没有导入依然可以使用
    onMounted:{
      num.value=100
    }
    function reduce(){
      num.value-=1
    }
    function add(){
      num.value+=1
    }
</script>

<style scoped lang="scss">
.example{
  display: flex;
  height: 25px;
  line-height: 25px;
  justify-content: center;
  button{
    width: 50px;
    height: 25px;
  }
  div{
    padding: 0 10px;
  }
}
</style>
