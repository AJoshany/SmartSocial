<template>
  <nav>
    <NuxtLink v-for="(item,index) in navItems" :key="index" :to="item.path">
      {{ item.title }}
    </NuxtLink>
  </nav>
</template>

<script setup>
  const navItems = [
    {title:'امکانات' , path:'/'},
    {title:'تعرفه ها' , path:'/'},
    {title:'بلاگ' , path:'/'},
    {title:'تماس با ما' , path:'/'},
  ]
</script>

<style>

</style>