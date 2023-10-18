<template>
    <div class="w-[24%] flex flex-col justify-center items-center">
        <p>{{title}}</p>
        <div>
            <slot />
        </div>
        <p class="w-full flex items-center gap-2 justify-center">
            <span v-if="increased" class="text-[#1CB647]">
                <font-awesome-icon  icon="fa-solid fa-chevron-up" class="fa-1x"/>
            </span>
            <span v-if="!increased" class="text-[#FF6B6B]">
                <font-awesome-icon  icon="fa-solid fa-chevron-down" class="fa-1x"/>
            </span>
            <span v-if="increased">Increased</span>
            <span v-if="!increased">Decreased</span>
        </p>
    </div>
</template>

<script lang="ts" setup>
const props = defineProps(['title', 'increased'])
</script>

<style lang="scss" scoped>


</style>