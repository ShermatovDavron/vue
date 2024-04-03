<script setup>

import Input from "@/components/icons/Input.vue";
</script>

<template>
<div class="search">
  <input type="text" placeholder="Search">
</div>
</template>

<style scoped>
.search{
  input{
    width: 285px;
    height: 48px;
    border-radius: 71px;
    border: 1px solid #EFEFEF;
    padding-left: 30px;
    &::placeholder{
      font-size: 14px;
      color: #70737C;
      font-family:sans-serif ;
    }
  }
}
</style>