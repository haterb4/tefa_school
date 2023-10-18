<template>
    <div class="w-[150px] flex flex-col justify-center items-start">
        <div class="flex flex-col justify-center items-center gap-2 h-[80px]">
            <div class="w-[60px] h-[60px] border rounded-full flex justify-center items-center">
                <img :src="image" alt="">
            </div>
            <div class="w-full h-[20px]">
                <h2 class="text-center">{{ title }}</h2>
            </div>
        </div>
    </div>
</template>

<script lang="ts" setup>
    const props = defineProps(['image', 'title']);
</script>

<style lang="scss" scoped>

</style>