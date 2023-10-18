<template>
    <div class="w-full h-screen flex flex-col justify-between items-center overflow-hidden bg-[url(/assets/images/tree.jpg)] bg-no-repeat bg-cover">
        <AppHeader />
        <div class="w-full h-[calc(100%-280px)] m-auto mx-0 mt-0 mb-0 bg-white">
            <slot />
        </div>
        <AppFooter />
    </div>
</template>

<script setup>

</script>

<style lang="scss" scoped>


</style>