<template>
    <div class="w-full h-screen overflow-hidden bg-[url(/assets/images/tree.jpg)] bg-no-repeat bg-cover">
        <div class="bg-[rgba(0,167,218,0.7)] w-full h-full flex flex-col justify-between items-center">
            <div class="w-full h-[calc(100%-80px)] flex flex-col justify-end items-center pt-8 pb-16">
                <slot></slot>
            </div>
            <div class="h-[80px] w-full px-20 flex flex-col justify-between items-center text-white text-lg">
                <div class="w-full flex justify-between items-center">
                    <nuxt-link to="/" class="font-bold">
                        Contact Us
                    </nuxt-link>
                    <nuxt-link to="/" class="font-bold">
                        Go to TEFA Afrik
                    </nuxt-link>
                </div>
                <p>Copyright &copy; TEFA {{ new Date().getFullYear() }}</p>
            </div>
        </div>
    </div>
</template>