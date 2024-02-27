<script setup lang="ts">
defineProps<{
 lg?: boolean;
}>();
</script>
<template>
 <div class="flex items-center gap-4 select-none">
  <div
   class="w-[40px] h-[40px] sm:w-[75px] sm:h-[75px] md::w-[100px] md::h-[100px]"
  >
   <img
    src="../assets/logo.jpeg"
    alt="Vue logo"
    :width="lg ? '100px' : '50px'"
    :height="lg ? '100px' : '50px'"
   />
  </div>
  <h1
   class="text-4xl sm:text-7xl bg-clip-text text-transparent bg-gradient-to-br from-slate-500 via-neutral-100 to-slate-500 font-bold"
   :class="{ 'md:text-8xl': lg }"
  >
   MoonTracker
  </h1>
 </div>
</template>
