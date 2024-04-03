<script setup>
import Card from "@/components/icons/Card.vue";
import {ref} from "vue";

const data = ref([
  {
    id:0,
    title: "Seedra Cilantro Seeds for Planting Indoor and Outdoor",
    price: Math.floor(Math.random() * 30)
  },
  {
    id:1,
    title: "Seedra Cilantro Seeds for Planting Indoor and Outdoor",
    price: Math.floor(Math.random() * 30)
  },
  {
    id:2,
    title: "Seedra Cilantro Seeds for Planting Indoor and Outdoor",
    price: Math.floor(Math.random() * 30)
  },
  {
    id:3,
    title: "Seedra Cilantro Seeds for Planting Indoor and Outdoor",
    price: Math.floor(Math.random() * 30)
  },
  {
    id:4,
    title: "Seedra Cilantro Seeds for Planting Indoor and Outdoor",
    price: Math.floor(Math.random() * 30)
  },
  {
    id:5,
    title: "Seedra Cilantro Seeds for Planting Indoor and Outdoor",
    price: Math.floor(Math.random() * 30)
  }
])
function deleteArr(id){
  delete data.value[id]
}
</script>

<template>
  <div class="container">
    <div class="cards">
      <div v-for="dataItem in data" >
        <Card v-bind="dataItem" @countInc="deleteArr" />
      </div>
    </div>
  </div>
</template>

<style scoped>
.cards {
  box-sizing: border-box;
 margin: 20px auto;
  display: flex;
  justify-content: space-around;
  align-items: center;
  flex-wrap: wrap;
}
</style>