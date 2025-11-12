<template>
  <nav class="flex gap-10 text-2xl">
    <NuxtLink v-for="(item,index) in navItems" :key="index" :to="item.path"
    class="hover:text-primary-500 transition-all px-4"
    >
      {{ item.title}}
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