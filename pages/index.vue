<template>
    <div class="w-[550px] h-[80%] min-h-[300px] bg-white rounded-lg flex flex-col justify-center items-center text-[#00A7DA] relative overflow-hidden">
        <div class="text-center">
            <h1 class="font-extrabold text-3xl">Welcome</h1>
            <p class="font-bold text-xl">Start Learning via Evaluation</p>
        </div>
        <div class="flex flex-col items-center">
            <div class="py-8 space-y-4">
                <AuthInput label="Password" placeholder="Use at least 6 characters" type="password"/>
                <AuthInput label="Username" placeholder="Username" type="text" />
                <AuthSelect label="Change School?" placeholder="Choose your school" :options="schools" />
            </div>
            <button
                @click="handleSubmit"
                class="px-12 py-2 text-white bg-[#00A7DA] rounded-[25px] text-xl"
            >
                Login
            </button>
        </div>
        <div class="absolute h-[150px] w-[150px] -bottom-8 -right-8">
            <img src="/icons/School_Icon_1.png" alt="">
        </div>
    </div>
</template>

<script lang="ts" setup>
import { ref } from "vue"
const router = useRouter()
const schools = ref([
    {
        index: 1,
        name: 'School 1'
    },
    {
        index: 2,
        name: 'School 2'
    },
    {
        index: 3,
        name: 'School 3'
    },
    {
        index: 4,
        name: 'School 4'
    },
    {
        index: 5,
        name: 'School 5'
    },
    {
        index: 6,
        name: 'School 6'
    },
])
const handleSubmit = async() => {
    router.push('/home')
}
definePageMeta({
    layout: "authentication",
});
</script>

<style lang="scss" scoped>


</style>