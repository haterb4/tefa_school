<template>
    <div class="w-full my-2">
        <div class="w-full flex flex-col items-start">
            <button @click="toggleOpen" class="font-bold text-xl w-full flex justify-between items-center">
                <span>{{ title }}</span>
                <font-awesome-icon icon="fa-solid fa-chevron-down" class="fa-1x"/>
            </button>
            <div v-if="isOpen" class="py-2 px-2">{{ content }}</div>
        </div>
    </div>
</template>

<script lang="ts" setup>
import { ref } from "vue"
const props = defineProps(['title', 'content'])
const isOpen = ref(false)

const toggleOpen = () => {
    isOpen.value = !isOpen.value
}
</script>

<style lang="scss" scoped>


</style>