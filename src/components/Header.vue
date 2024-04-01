<script setup>

import Button from "@/components/icons/Button.vue";
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
      <Button className="btn-icon-card"/>
    </nav>
  </div>
</template>

<style scoped>
.nav {
  display: flex;
  justify-content: space-between;
  align-items: center;
  width: 1440px;
  height: 72px;
  box-shadow: 12px 0 #CFCFCF40;
  .nav_list{
    display: flex;
    list-style: none;
    a{
      text-decoration: none;
      color:#70737C ;
      font-weight: 400px;
    }
  }
}
</style>