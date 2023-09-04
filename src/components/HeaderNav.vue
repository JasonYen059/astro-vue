<template>
    <nav class="container mx-auto flex flex-row justify-between py-5 border-b-4">
        <a class="logo text-2xl" href="/">YEN</a>
        <ul class="flex flex-row">
            <li v-for="link in navList" :key="link.link" class=" text-lg px-3">
                <a :href="link.link">{{ link.text }}</a>
            </li>
        </ul>
    </nav>
</template>

<script setup>
// import { ref } from 'vue';

const props = defineProps({
    titleName: String
});
const navList = [
    { text: 'ABOUT', link: 'about' },
    { text: 'WORK', link: 'work' },
]

</script>