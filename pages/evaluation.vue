<template>
    <div class="w-full h-full flex">
        <div class="h-full w-full px-4 overflow-hidden md:w-[20%] flex flex-col justify-center items-center ">
            <div class="w-[70%]">
                <div class="text-center py-4">
                    <p>16 Days left</p>
                </div>
                <ProgressBar foreground="bg-cyan-800" background="bg-cyan-50" fill="w-[50%]"/>
            </div>
            <LeftLibrary />
        </div>
        <div class="w-full md:w-[80%] h-full overflow-hidden px-8">
            <div class="w-full h-[100px] flex justify-center items-center gap-4">
                <EvalItemCard
                    v-for="mater in maters"
                    :key="mater.title"
                    :title="mater.title"
                    :image="mater.image"
                />
            </div>
            <div class="h-[calc(100%-100px)] w-full pt-4 flex flex-col items-center justify-center gap-3">
                <EvalRow />
                <EvalRow />
                <EvalRow />
                <EvalRow />
            </div>
        </div>
    </div>
</template>

<script lang="ts" setup>
    import { ref } from 'vue';

    const maters = ref([
        {
            image: '/icons/Math_Icon_3.png',
            title: 'Mathematics'
        },
        {
            image: '/icons/Economics_Icon_4.png',
            title: 'Economics'
        },
        {
            image: '/icons/Computer_Science_Icon_1.png',
            title: 'Computer Science'
        },
        {
            image: '/icons/Statistics_Icon_2.png',
            title: 'Pure Mathematic and Statistics'
        },
        {
            image: '/icons/Physics_Icon_1.png',
            title: 'Physics'
        },
        {
            image: '/icons/Language_Icon_1.png',
            title: 'English'
        },
        {
            image: '/icons/Biology_Icon_1.png',
            title: 'Biology'
        },
        {
            image: '/icons/Chemistry_Icon_1.png',
            title: 'Chemistry'
        },
    ])
</script>

<style lang="scss" scoped>


</style>