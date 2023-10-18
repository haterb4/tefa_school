<template>
    <div class="w-full h-full">
      <div class="w-full h-[30px] border-b py-[2px] px-4 border-[#007194] flex items-center gap-3">
        <img v-if="prefix" :src="prefix" alt="" class="h-full w-[30px]">
        <h1>{{ title }}</h1>
        <img v-if="suffix" :src="suffix" alt="" class="h-full w-[30px]">
      </div>
      <div class="w-full h-[calc(100%-30px)] px-4 flex flex-col justify-center items-start">
        <slot />
      </div> 
    </div>
</template>

<script lang="ts" setup>
const props = defineProps(['suffix', 'title', 'prefix'])
</script>

<style lang="scss" scoped>


</style>