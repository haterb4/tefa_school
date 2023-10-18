<template>
    <nuxt-link @click="$emit('activate')" :to="menu.href" :class="[active ? 'bg-white text-[#239ad6]' : 'bg-[#239ad6] text-white', 'px-3 hover:bg-white hover:text-[#239ad6] rounded-[25px] flex items-center gap-3 py-2']">
        <font-awesome-icon :icon="icon" class="fa-1x"/>
        <span>{{ menu.title }}</span>
    </nuxt-link>
</template>

<script setup>
    const props = defineProps(['menu', 'active', 'icon'])
    console.log(props.iconName)
</script>

<style lang="scss" scoped>


</style>