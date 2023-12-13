<template>
  <div v-editable="blok" class="backdrop w-full h-[50vh] bg-green-100 flex justify-center align-center items-center">
    <h1 class="text-slate-700 font-bold font-serif text-center text-4xl mt-40" v-html="title"></h1>
  </div>
</template>

<script setup>
// defineProps({ blok: Object })
const props = defineProps({ blok: Object })
const title = computed(() => renderRichText(props.blok.title));
</script>
