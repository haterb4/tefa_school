<template>
    <div :class="'w-full h-[5px] rounded-[25px] ' +background">
        <div :class="['h-full rounded-[25px]', foreground, fill]"></div>
    </div>
</template>

<script lang="ts" setup>
    defineProps(['foreground', 'background', 'fill'])
</script>

<style lang="scss" scoped>


</style>