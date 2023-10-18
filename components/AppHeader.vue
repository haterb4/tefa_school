<template>
    <div class="w-full h-[180px] px-12 py-4 bg-[rgba(35,154,214,0.86)] text-white">
        <div class="w-full flex justify-between items-center">
            <h1 class="font-extrabold text-2xl">Francky Local Complex</h1>
            <p>Form 5</p>
            <div class="flex items-center gap-12">
                <h4>{{ new Date().toLocaleDateString() }}</h4>
                <div class="w-[60px] h-[100px] flex flex-col justify-center items-center">
                    <div class="w-[70px] h-[70px] rounded-full bg-white border-[#239ad6]">
                        <img class="h-full w-full rounded-full" src="/images/profile.jpg" alt="">
                    </div>
                    <h2 class="mb-1">Nehemia</h2>
                    <nuxt-link to="/admin/principal" class="flex gap-4">
                        <span>Profile</span>
                        <font-awesome-icon icon="fa-solid fa-user" />
                    </nuxt-link>
                </div>
            </div>
        </div>
        <Navbar />
    </div>
</template>

<script setup>

</script>

<style lang="scss" scoped>


</style>