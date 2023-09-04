<template>
    <div>
        {{ titleName }}
    </div>
</template>

<script setup>
// import { ref } from 'vue';

const props = defineProps({
    titleName:String
});

</script>

<style lang="scss" scoped>

</style>