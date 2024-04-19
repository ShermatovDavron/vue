<script setup>
import {computed} from "vue";

const props = defineProps({
  img_src:String,
  title:String,
  time:Date,
  desc:String,
})
const stars = computed(()=>{
  return Math.ceil(Math.random()*5)
})
</script>

<template>
  <div class="card">
      <div class="card__title">
        <img src="@/assets/img/star.svg" alt="">
        <div>
          <h2>{{props.title}}</h2>
          <time>{{props.time}}</time>
        </div>
      </div>
      <ul class="card__stars">
          <li v-for="star in stars">
            <img src="@/assets/img/star.svg" alt="*">
          </li>
      </ul>
      <div class="card__desc">
        {{props.desc}}
      </div>
  </div>
</template>

<style lang="scss" scoped>
.card{
  font-family: sans-serif;
  box-sizing: border-box;
  padding:50px 34px;
  width: 540px;
  height: max-content;
  border:1px solid #EFEFEF ;
  box-shadow: 0 4px 21px  #D1D1D140;
  border-radius: 12px;
  color: #1F2533;
  &__title{
    display: flex;
    justify-content: flex-start;
    align-items: center;
    img{
      border-image: 50%;
      width:64px;
      height: 64px;
    }
    div{
      margin-left: 20px;
      h2{
        font-size: 18px;
      }
      time{
        font-size: 14px;
        color: #70737C;
      }
    }
  }
  &__stars{
    display: flex;
    justify-content: flex-start;
    align-items: center;
    list-style: none;
    padding: 0;
  }
  &__desc{
    font-family: sans-serif;
    font-size: 15px;
    font-weight: 300;
  }
}
</style>