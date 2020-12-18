<template>
  <div class="home">
    <example/>
    <example2 :msg="msg"/>
    <example3 :ref="(ref)=>{example3Ref=ref}"/>
    <example4/>
    <example5/>
  </div>
</template>

<script setup>
import example from '@/components/example.vue'
import example2 from '@/components/example2.vue'
import example3 from '@/components/example3.vue'
import example4 from '@/components/example4.vue'
import example5 from '@/components/example5.vue'
import { ref } from "vue";
let msg=ref('Welcome to Your Vue.js App')
let example3Ref=ref(null)
console.log(example3Ref)
</script>
