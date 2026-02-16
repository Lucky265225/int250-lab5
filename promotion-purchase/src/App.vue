<script setup>
import Card from './Card.vue';

</script>

<template>
  
  <div class="bg-[#283451] h-screen flex justify-center items-center gap-5">
    <Card 
      promotion = "BASIC"
      storage = "100GB"
      price = "$1.99/month"
    />
    <Card
      promotion = "STANDARD"
      storage = "200GB"
      price = "$3.99/month"
      isPopular = true
    />
    <Card
      promotion = "PREMIUM"
      storage = "2TB"
      price = "$8.99/month"
    />
  </div>

</template>

<style scoped></style>
