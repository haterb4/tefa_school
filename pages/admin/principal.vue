<template>
    <div class="w-full py-2 flex justify-between items-center">
        <div class="min-w-[300px] w-[24%] h-[300px] border rounded-md border-[#007194]">
            <ClassMasterFunctions title="Classmaster Functions">
                <button class="w-full py-1 flex items-center gap-4 my-1">
                    <span class="w-[25px] h-[25px] border border-[#007194] rounded-full flex justify-center items-center">
                        <font-awesome-icon icon="fa-solid fa-plus" />
                    </span>
                    <span>Add Teacher</span>
                </button>
                <button class="w-full py-1 flex items-center gap-4 my-1">
                    <span class="w-[25px] h-[25px] border border-[#007194] rounded-full flex justify-center items-center">
                        <font-awesome-icon icon="fa-solid fa-plus" />
                    </span>
                    <span>Add Class</span>
                </button>
                <button class="w-full py-1 flex items-center gap-4 my-1">
                    <span class="w-[25px] h-[25px] border border-[#007194] rounded-full flex justify-center items-center">
                        <font-awesome-icon icon="fa-solid fa-plus" />
                    </span>
                    <span>Add Subject</span>
                </button>
                <button class="w-full py-1 flex items-center gap-4 my-1">
                    <span class="w-[25px] h-[25px] rounded-full flex justify-center items-center">
                        <font-awesome-icon icon="fa-solid fa-graduation-cap" />
                    </span>
                    <span>Allocate Teachers to Subjects</span>
                </button>
                <button class="w-full py-1 flex items-center gap-4 my-1">
                    <span class="w-[25px] h-[25px] rounded-full flex justify-center items-center">
                        <font-awesome-icon icon="fa-solid fa-users" />
                    </span>
                    <span>Allocate Students to Classes</span>
                </button>
            </ClassMasterFunctions>
        </div>
        <div class="min-w-[300px] w-[24%] h-[300px] border rounded-md border-[#007194]">
            <ClassMasterFunctions title="Lowest 10 Rankings"></ClassMasterFunctions>
        </div>
        <div class="min-w-[300px] w-[24%] h-[300px] border rounded-md border-[#007194]">
            <ClassMasterFunctions title="Top 10 Rakings"></ClassMasterFunctions>
        </div>
        <div class="min-w-[300px] w-[24%] h-[300px] border rounded-md border-[#007194]">
            <ClassMasterFunctions title="Top 10 Rakings"></ClassMasterFunctions>
        </div>
    </div>
</template>

<script setup>
definePageMeta({
    layout: "admin",
});
</script>

<style lang="scss" scoped>


</style>