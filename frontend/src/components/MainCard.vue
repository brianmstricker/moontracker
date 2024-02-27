<script setup lang="ts">
defineProps<{
 title: string;
 image: string;
 orange?: boolean;
 white?: boolean;
 emerald?: boolean;
 amber?: boolean;
}>();
</script>

<template>
 <div
  class="bg-black p-4 rounded-2xl shadow-md border"
  :class="{
   'shadow-orange-500 border-orange-500': orange,
   'shadow-white border-white': white,
   'shadow-emerald-500 border-emerald-500': emerald,
   'shadow-amber-400 border-amber-400': amber,
  }"
 >
  <div class="flex items-center gap-2">
   <img :src="image" :alt="title" class="w-8 h-8" />
   <h2 class="text-4xl">{{ title }}</h2>
  </div>
  <p>content</p>
 </div>
</template>
