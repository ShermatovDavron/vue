<script setup>
import SectionCard from "@/components/icons/SectionCard.vue";
import { ref} from "vue";



const data = ref([
  {
    id:0,
    title:"Carla Samantoes-Diego1",
    time:"12.09.2021",
    desc:"SEEDRA Spinach Seeds - contains 600 seeds in 2 Packs and professional instructions created by PhD Helga George\n" +
        "Be sure of our quality - the freshest batches of this season. Non-GMO, Heirloom - our seeds were tested and have the best germination ratings. ",
    img_src:'icon'
  },
  {
    id:1,
    title:"Carla Samantoes-Diego2",
    time:"12.09.2021",
    desc:"SEEDRA Spinach Seeds - contains 600 seeds in 2 Packs and professional instructions created by PhD Helga George\n" +
        "Be sure of our quality - the freshest batches of this season. Non-GMO, Heirloom - our seeds were tested and have the best germination ratings. ",
    img_src:'icon'
  },
  {
    id:2,
    title:"Carla Samantoes-Diego3",
    time:"12.09.2021",
    desc:"SEEDRA Spinach Seeds - contains 600 seeds in 2 Packs and professional instructions created by PhD Helga George\n" +
        "Be sure of our quality - the freshest batches of this season. Non-GMO, Heirloom - our seeds were tested and have the best germination ratings. ",
    img_src:'icon'
  },
  {
    id:3,
    title:"Carla Samantoes-Diego4",
    time:"12.09.2021",
    desc:"SEEDRA Spinach Seeds - contains 600 seeds in 2 Packs and professional instructions created by PhD Helga George\n" +
        "Be sure of our quality - the freshest batches of this season. Non-GMO, Heirloom - our seeds were tested and have the best germination ratings. ",
    img_src:'icon'
  },
  {
    id:4,
    title:"Carla Samantoes-Diego5",
    time:"12.09.2021",
    desc:"SEEDRA Spinach Seeds - contains 600 seeds in 2 Packs and professional instructions created by PhD Helga George\n" +
        "Be sure of our quality - the freshest batches of this season. Non-GMO, Heirloom - our seeds were tested and have the best germination ratings. ",
    img_src:'icon'
  },
  {
    id:5,
    title:"Carla Samantoes-Diego6",
    time:"12.09.2021",
    desc:"SEEDRA Spinach Seeds - contains 600 seeds in 2 Packs and professional instructions created by PhD Helga George\n" +
        "Be sure of our quality - the freshest batches of this season. Non-GMO, Heirloom - our seeds were tested and have the best germination ratings. ",
    img_src:'icon'
  },
  {
    id:6,
    title:"Carla Samantoes-Diego7",
    time:"12.09.2021",
    desc:"SEEDRA Spinach Seeds - contains 600 seeds in 2 Packs and professional instructions created by PhD Helga George\n" +
        "Be sure of our quality - the freshest batches of this season. Non-GMO, Heirloom - our seeds were tested and have the best germination ratings. ",
    img_src:'icon'
  }
])



</script>

<template>
  <div class="container section">
    <h1>What out clients say</h1>
    <swiper
        :pagination="pagination" :modules="modules" class="mySwiper"
    >
        <swiper-slide v-for="item in data" style="margin: 10px;">
          <SectionCard
                       :key="item.id"
                       :title=item.title
                       :desc="item.desc"
                       :time="item.time"
                       :img_src="item.img_src"
          />
        </swiper-slide>
    </swiper>
    <ul class="section__btn" >
      <li v-for="num in data.length"  @click=""></li>
    </ul>
  </div>
</template>

<style scoped lang="scss">
.section{
  h1{
    text-align: center;
    font-size: 36px;
    color:#1F2533;
    font-family: 'Lexend',sans-serif;
  }
  &__item{
    display: flex;
    width: max-content;
    height: 450px;
    position: relative;
    div{
      margin-top: 110px;
      margin-left: 60px;
    }
  }
  &__btn{
    margin: 20px;
    display: flex;
    justify-content: center;
    align-items: center;
    list-style: none;
    li{
      margin: 0 10px;
      width:60px;
      height: 6px;
      background-color: rgba(53, 151, 64, 0.43);
      border-radius: 30px;
      &:hover{
        background-color: rgba(5, 209, 28, 0.43);
      }
    }
  }
.mySwiper{
  display: flex;
  flex-wrap: wrap;
  justify-content: center;
  align-items: center;
}

}
.active{
  background-color: #359740;
}
</style>