<script setup>
defineProps(['type','placeholder','label','place_color'])
</script>

<template>
  <div class="input">
    <label >{{label}}</label>
    <input :type="type" :placeholder="placeholder">
    <slot></slot>
  </div>
</template>

<style scoped>
.input{
  display: flex;
  justify-content: flex-start;
  flex-direction: column;
  line-height:20px;
  label{
    color: #70737C;
    font-weight: 400;
    font-size: 14px;
  }
  input{
    border-radius: 4px;
    width: 350px;
    height: 56px;
    border: 1px solid #EFEFEF;
    &:hover{
      border: 1px solid #EFEFEF ;
      box-shadow:0 1px 6px 0 #00000052 ;
    }
    ::placeholder{
      color: #70737C;
    }
    &:focus,&:active{
      border: 1px solid #EFEFEF ;
      box-shadow:0 1px 6px 0 #00000052 ;
    }

  }
}
</style>