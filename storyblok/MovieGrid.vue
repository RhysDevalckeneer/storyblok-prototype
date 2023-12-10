<template>
    <div v-editable="blok" class="max-w-7xl mx-auto">
        <h2 class="font-bold text-2xl">{{blok.title}}</h2>
        <div class="grid grid-cols-6 gap-4">
            <StoryblokComponent
            v-for="blok in blok.columns"
            :key="blok._uid"
            :blok="blok"
            />
        </div>
    </div>
</template>

<script setup>
defineProps({ blok: Object })
</script>
