<script setup>
import {ref} from "vue";
import BlogCard from "@/components/icons/BlogCard.vue";
import Button from "@/components/icons/Button.vue";

const data = ref([
  {
    date: '11-09-2002',
    title: "How to plant spinach correctly in winter",
    text: "In most areas, successive sowing can be done from early spring until early winter, but more often during hotter months..."
  },
  {
    date: '11-09-2002',
    title: "How to plant spinach correctly in winter",
    text: "In most areas, successive sowing can be done from early spring until early winter, but more often during hotter months..."
  },
  {
    date: '11-09-2002',
    title: "How to plant spinach correctly in winter",
    text: ""
  },
  {
    date: '11-09-2002',
    title: "How to plant spinach correctly in winter",
    text: ""
  }
])


</script>

<template>

  <div class="container blog">
    <div class="blog_title">
      <h1>Our Blog.</h1>
      <Button class-name="btn-white" style="font-size: large">go to our blog</Button>
    </div>
    <div class="blog_cards">
      <div>
        <BlogCard :data="data[0]" style="width:730px " class="blog_column"/>
        <div class="blog_card">
          <BlogCard :data="data[2]" style="width: 300px"/>
          <BlogCard :data="data[3]" style="width: 300px"/>
        </div>
      </div>
      <BlogCard :data="data[1]" style="width: 400px; height:500px"/>
    </div>
  </div>

</template>

<style scoped>
.blog {

  .blog_title {
    display: flex;
    justify-content: space-between;
    align-items: center;
    padding: 10px;
    margin-bottom: 20px;
    h1 {
      color: #1F2533;
      font-weight: 600;
      font-family: sans-serif;
    }
  }
  .blog_cards {
    height: 600px;
    padding: 10px;
    display: flex;
    align-items: center;
    justify-content: space-between;
    div{
      width: 830px;
      .blog_card{
        height: 300px;
        display: flex;
        justify-content: space-around;
        align-items: flex-start;
      }
    }
  }
}
.blog_column{
  margin-bottom: 20px;
}
</style>