<template>
    <div v-editable="blok" class="h-48 w-30 relative rounded">
        <img :src="blok.poster.filename" :alt="blok.title" class="w-full h-full object-cover"/>
        <span class="px-2 py-1 bg-slate-400 text-xs text-white font-bold absolute top-1 right-1 rounded-md">{{blok.score}}</span>
        <div class="w-full p-2 bg-gradient-to-t from-white to-transparent absolute bottom-0 left-0">
            <p class="font-bold">{{blok.title}}</p>
        </div>
    </div>
  </template>
  
  <script setup>
  defineProps({ blok: Object })
  </script>
  