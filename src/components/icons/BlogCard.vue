<script setup>
import Button from "@/components/icons/Button.vue";

const props=defineProps(
  {
    data:Object,
  }
)

</script>

<template>
<div class="container card" >
  <time>
    {{props.data.date}}
  </time>
  <h2>
    {{props.data.title}}
  </h2>
  <p>
   {{props.data.text}}
  </p>
  <Button class-name="btn-white" style="font-size: large">Read</Button>
</div>
</template>

<style scoped>
.card{
  border-radius: 12px;
  padding: 30px;
  box-sizing: border-box;
  background-color:#EAF1EB ;
}
</style>