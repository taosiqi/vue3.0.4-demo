<template>
  <!-- 案例2-->
  <h1>{{props.msg}}</h1>
</template>

<script setup>
    import {defineProps } from "vue";
    const props = defineProps({
      msg: {
        type: String,
      },
    });
</script>


