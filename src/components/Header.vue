<script setup>

import Button from "@/components/icons/Button.vue";
import Search from "@/components/icons/Search.vue";
</script>

<template>
  <div class="container">
    <nav class="nav">
      <div class="nav_logo">
        <a href="#">
          <img src="@/assets/img/logo.png" alt="Logo">
        </a>
      </div>
      <ul class="nav_list">
        <li><a href="#">ALL PRODUCTS</a></li>
        <li><a href="#">ABOUT SEEDRA</a></li>
        <li><a href="#">OUR BLOG</a></li>
        <li><a href="#">CONTACT</a></li>
      </ul>
      <Search/>
      <Button class-name="btn-icon-card" btn-font-size="50"/>
    </nav>
  </div>
</template>

<style scoped>
.nav {
 margin: 0 auto;
  box-sizing: border-box;
  display: flex;
  justify-content: space-between;
  align-items: center;
  height: 72px;
 box-shadow: 0 1px 1px 0 ;
  padding: 0 10px;
  .nav_list{
    display: flex;
    list-style: none;
    li{
      padding: 2px 10px;
      border-right: 1px solid #EFEFEF;
      &:nth-last-child(-n+1){
        border: none;
      }
      a{
        text-decoration: none;
        color:#70737C ;
        font-weight: 400;
      }
    }
  }
}
</style>