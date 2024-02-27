<script setup lang="ts">
import MainCard from "../components/MainCard.vue";
import Title from "../components/Title.vue";
import bitcoin from "../assets/bitcoin.png";
import bnb from "../assets/bnb.png";
import ethereum from "../assets/ethereum.png";
import tether from "../assets/tether.png";
</script>
<template>
 <div class="w-screen h-screen relative overflow-hidden">
  <div id="stars" />
  <div id="stars1" />
  <div id="stars2" />
  <div id="stars3" />
  <div class="w-full h-full flex flex-col items-center relative">
   <section class="z-[2] absolute top-[10%] sm:top-[20%]">
    <Title lg />
   </section>
   <section
    class="z-[2] w-full mx-auto max-w-5xl absolute top-[25%] sm:top-[40%] flex justify-center"
   >
    <div class="grid grid-cols-1 sm:grid-cols-2 lg:grid-cols-4 gap-4">
     <MainCard title="Bitcoin" :image="bitcoin" orange />
     <MainCard title="Ethereum" :image="ethereum" white />
     <MainCard title="Tether" :image="tether" emerald />
     <MainCard title="BNB" :image="bnb" amber />
    </div>
   </section>
  </div>
 </div>
</template>
