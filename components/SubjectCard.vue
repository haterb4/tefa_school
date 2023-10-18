<template>
    <div class="w-full flex flex-col justify-center items-center text-[#00A7DA]">
        <div class="w-full relative border h-[120px] rounded-[12px]">
            <div class="w-full h-full flex flex-col justify-center items-center px-4">
                <div class="w-full flex justify-between items-start">
                    <h1 class="font-bold text-lg w-[180px]">{{ subject.title }}</h1>
                    <div class="h-[90px] w-[90px] bg-orange-50 rounded-full flex justify-center items-center">
                        <img :src="subject.image" alt="">
                    </div>
                </div>
            </div>
            <div class="absolute top-1 left-1 w-[10px] h-[10px] rounded-full border" />
        </div>
        <div class="w-full flex justify-between items-start">
            <div>
                <p>Rank: {{subject.studentRank}}th/{{ subject.allStudents}}</p>
                <p>Evaluations: {{ subject.evaluation}}</p>
                <p>Progress {{ subject.progress }}%</p>
            </div>
            <div class="text-right">
                <p class="space-x-2">
                    <span><font-awesome-icon icon="fa-solid fa-graduation-cap" class="fa-1x"/></span> 
                    <span>{{ subject.teacher }}</span>
                </p>
                <p>Students present: {{subject.presentStudents}}/{{ subject.allStudents}}</p>
            </div>
        </div>
    </div>
</template>

<script lang="ts" setup>
const props = defineProps(['subject'])
</script>

<style lang="scss" scoped>


</style>