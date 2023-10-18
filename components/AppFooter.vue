<template>
    <Footer class="w-full h-[100px] py-12 flex flex-col sm:flex-row gap-4 sm:gap-0 justify-between items-center bg-[rgba(35,154,214,0.76)] px-12">
        <div class="flex gap-8">
            <div class="w-[50px] h-[50px] rounded-full text-white border-[#239ad6] flex justify-center items-center bg-green-600">
                <font-awesome-icon icon="fa-brands fa-whatsapp" class="fa-2x"/>
            </div>
            <div class="w-[50px] h-[50px] rounded-full bg-white border-[#239ad6] text-[#239ad6] flex flex-col justify-center items-center">
                <span class="font-bold text-xs">TEFA</span>
                <span class="font-bold text-xs">Afrik</span>
            </div>
        </div>
        <div>
            <div class="bg-white w-full sm:w-[250px] rounded-[25px] border-[#239ad6] outline-none">
                <input
                    type="text"
                    class="w-full h-[40px] rounded-[25px] px-2"
                    placeholder="Ask me anything..."
                />
            </div>
        </div>
    </Footer>
</template>

<script setup>
    
</script>

<style lang="scss" scoped>


</style>