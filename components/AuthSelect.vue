<template>
    <div class="flex flex-col justify-center items-center space-y-3">
        <label :for="label" class="text-xl font-bold">{{ label }}</label>
        <select
            :id="label"
            class="w-[300px] border-2 border-[#00A7DA] h-[50px] rounded-[25px] px-3 outline-0"
        >
            <option :value="placeholder">{{ placeholder }}</option>
            <option v-for="option in options" :key="option.index" :value="option.name">{{ option.name }}</option>
        </select>
    </div>
</template>

<script lang="ts" setup>
const props = defineProps(['label', 'placeholder', 'options'])
</script>

<style lang="scss" scoped>


</style>