<script setup>
import ContentPicture from './components/ContentPicture.vue';
import Header from './components/Header.vue';
import Navbar from './components/Navbar.vue';

</script>

<template>

  <div class="min-h-screen">
    <div class="flex-col w-[60%] m-auto">
      <Navbar/>
      <Header/>
      <ContentPicture/>
    </div>
  </div>
  
</template>

<style scoped></style>
