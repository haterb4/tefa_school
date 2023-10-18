<template>
    <nav class="w-full flex justify-center items-center">
        <div class="flex items-center justify-center gap-8">
            <button class="w-[40px] h-[40px] rounded-full bg-white text-[#239ad6] flex items-center justify-center">
                <font-awesome-icon icon="fa-solid fa-angles-left" class="fa-1x"/>
            </button>
            <div class="flex gap-4">
                <NavItem
                 v-for="menu in menus"
                :key="menu.id" :menu="menu"
                @activate="setActiveMenu(menu.id)"
                :active="activeMenu === menu.id ? true : false"
                :icon="menu.icon"
            />
            </div>
            <button class="w-[40px] h-[40px] rounded-full bg-white text-[#239ad6] flex items-center justify-center">
                <font-awesome-icon icon="fa-solid fa-angles-right" class="fa-1x"/>
            </button>
        </div>
    </nav>
</template>

<script setup lang="ts">
    import { ref } from 'vue'
    const activeMenu = ref(0)
    const menus = ref([
        {
            id: 0,
            title: 'Home',
            icon: ['fas', 'calendar-days'],
            href: '/'
        },
        {
            id: 1,
            title: 'Evaluation',
            icon: ['fas', 'file-signature'],
            href: '/evaluation'
        },
        {
            id: 2,
            title: 'Corrections',
            icon: ['fas', 'graduation-cap'],
            href: '/correction'
        },
        {
            id: 3,
            title: 'Progress',
            icon: ['fas', 'chart-simple'],
            href: '/progress'
        },
    ])
    const setActiveMenu = (menuId: number) => {
        activeMenu.value = menuId
    }
</script>

<style lang="scss" scoped>


</style>