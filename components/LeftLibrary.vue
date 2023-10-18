<template>
    <div class="w-full h-full flex justify-center items-center">
        <div class="flex flex-col justify-center items-center">
        <div class="flex flex-col items-center">
            <div class="w-[100px] h-[100px] rounded-full flex justify-center items-center text-red-500">
                <img src="/icons/Book_Icon_1.png" alt="">
            </div>
            <p class="mt-3">Our Library</p>
            <nuxt-link to="/library" class="px-4 py-1 border rounded-[25px] w-[180px] text-center">Browse...</nuxt-link>
        </div>
        <div class="text-center pt-2">
            <p><span class="font-extrabold">4890</span> Questions</p>
            <p><span class="font-extrabold">500</span> Video courses</p>
            <p><span class="font-extrabold">670</span> Course notes</p>
            <p><span class="font-extrabold">200</span> Books</p>
        </div>
        </div>
    </div>
</template>

<script lang="ts" setup>

</script>

<style lang="scss" scoped>


</style>