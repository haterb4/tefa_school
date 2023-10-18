<template>
    <div class="flex flex-col justify-center items-center space-y-3">
        <label :for="label" class="text-xl font-bold">{{ label }}</label>
        <input
            :type="type"
            :placeholder="placeholder"
            :id="label"
            class="w-[300px] border-2 border-[#00A7DA] h-[50px] rounded-[25px] px-3 outline-0"
        />
    </div>
</template>

<script lang="ts" setup>
const props = defineProps(['label', 'placeholder', 'type'])
</script>

<style lang="scss" scoped>


</style>