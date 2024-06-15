<script setup>
import {ref} from "vue";
import Button from "@/components/icons/Button.vue";

const price = ref(12.56)
const priceOld = ref(15.56)
</script>

<template>
<div class="container">
  <div class="box">
    <h2>SEEDRA Basil Seeds for Indoor and Outdoor Planting</h2>
    <p>Be sure of our quality - the freshest batches of this season. Non-GMO, Heirloom - our seeds were tested and have the best germination ratings. Your easy growing experience is our guarantee</p>
    <div class="prices">
      <h2 >${{price}}</h2>
      <h3>${{priceOld}}</h3>
    </div>
    <div class="buttons">
      <Button class-name="btn-green" style="font-size: 20px">Add card</Button>
      <Button class-name="btn-white" style="font-size: 20px">Discover</Button>
    </div>
  </div>
</div>
</template>

<style scoped>
.box{
  margin: 0 auto;
  box-sizing: border-box;
  background-color:#EAF1EB ;
  background-image: url("@/assets/img/seedra.png");
  background-position-x: right;
  background-position: center right;
  padding: 50px 100px;
  background-repeat: no-repeat;
  h2{
    color: #1F2533;
    font-weight: 600;
    font-size: 48px;
    line-height: 54px;
    font-family: sans-serif;
    width: 650px;
  }
  p{
    color: #1F2533;
    font-weight: 300;
    font-size: 16px;
    line-height: 28px;
    font-family: sans-serif;
    width: 650px;
  }
  .prices{
    display: flex;
    color:#1F2533 ;
    font-weight: 600;
    h2{
      font-size: 42px;
      margin-right: 20px;
    }
    h3{
      font-size: 22px;
      text-decoration:#70737C;
      text-decoration-line: line-through;
    }
  }
  .buttons{
    display: flex;
    Button{
      margin-right: 20px;
    }
  }

}
</style>