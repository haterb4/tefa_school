<template>
    <div class="w-full h-screen flex justify-between items-start overflow-hidden text-white relative">
        <div class="h-full overflow-hidden w-[25%] py-4 bg-[#007194] flex flex-col justify-between items-center">
            <div class="flex justify-start items-center gap-4">
                <div class="h-[80px] w-[80px] border rounded-full bg-white flex justify-center items-center">
                    <img class="h-full w-full rounded-full" src="/icons/School_Icon_1.png" alt="">
                </div>
                <div>
                    <h1 class="font-bold text-2xl">Franky Local Complex</h1>
                    <h2 class="font-bold text-2xl">Year 2023</h2>
                </div>
            </div>
            <div class="w-full h-[calc(100%-150px)] overflow-hidden py-12">
                <div class="h-full w-full overflow-y-scroll custom-nav-hidden space-y-8">
                    <div class="w-full flex flex-col items-start px-12">
                        <DropDown title="Pick a Class">
                            <form class="space-y-3">
                                <div class="flex items-center gap-2">
                                    <div class="w-[20px] h-[20px] rounded-full">
                                        <input type="radio" name="class1" id="class1" class="w-full h-full rounded-full">
                                    </div>
                                    <label for="class1"> choose class 1</label>
                                </div>
                                <div class="flex items-center gap-2">
                                    <div class="w-[20px] h-[20px] rounded-full">
                                        <input type="radio" name="class1" id="class2" class="w-full h-full rounded-full">
                                    </div>
                                    <label for="class2"> choose class 1</label>
                                </div>
                                <div class="flex items-center gap-2">
                                    <div class="w-[20px] h-[20px] rounded-full">
                                        <input type="radio" name="class1" id="class3" class="w-full h-full rounded-full">
                                    </div>
                                    <label for="class3"> choose class 1</label>
                                </div>
                                <div class="flex items-center gap-2">
                                    <div class="w-[20px] h-[20px] rounded-full">
                                        <input type="radio" name="class1" id="class4" class="w-full h-full rounded-full">
                                    </div>
                                    <label for="class4"> choose class 1</label>
                                </div>
                            </form>
                        </DropDown>
                        <DropDown title="Pick a Role">
                            <form class="space-y-3">
                                <div class="flex items-center gap-2">
                                    <div class="w-[20px] h-[20px] rounded-full">
                                        <input type="checkbox" name="class1" id="role1" class="w-full h-full rounded-full">
                                    </div>
                                    <label for="role1"> choose Role 1</label>
                                </div>
                                <div class="flex items-center gap-2">
                                    <div class="w-[20px] h-[20px] rounded-full">
                                        <input type="checkbox" name="class1" id="role2" class="w-full h-full rounded-full">
                                    </div>
                                    <label for="role2"> choose Role 2</label>
                                </div>
                                <div class="flex items-center gap-2">
                                    <div class="w-[20px] h-[20px] rounded-full">
                                        <input type="checkbox" name="class1" id="role3" class="w-full h-full rounded-full">
                                    </div>
                                    <label for="role3"> choose Role 3</label>
                                </div>
                                <div class="flex items-center gap-2">
                                    <div class="w-[20px] h-[20px] rounded-full">
                                        <input type="checkbox" name="class1" id="role4" class="w-full h-full rounded-full">
                                    </div>
                                    <label for="role4"> choose Role 4</label>
                                </div>
                            </form>
                        </DropDown>
                        <DropDown title="Pick a Teacher"></DropDown>
                        <DropDown title="Pick a Term"></DropDown>
                        
                    </div>
                    <div class="w-full">
                        <div class="flex justify-center items-center">
                            <span class="font-bold text-xl">Recent Activity</span>
                        </div>
                    </div>
                </div>
            </div>
            <div class="flex justify-center items-center gap-4 w-full">
                <input type="text" placeholder="ask me anything" class="py-1 rounded-[25px] px-2 h-[50px] w-[calc(100%-150px)] border-[#2E9ED9]">
                <button class="w-[50px] h-[50px] rounded-full text-white bg-[#1CB647]">
                    <font-awesome-icon icon="fa-brands fa-whatsapp" class="fa-2x"/>
                </button>
            </div>
        </div>
        <div class="h-full overflow-hidden w-[75%] py-2 px-4 flex flex-col justify-between items-center text-[#007194]">
            <div class="w-full h-[calc(100%-50px)] overflow-hidden">
                <div class="w-full h-[50px]">
                    <div class="w-full flex justify-end items-center">
                        <div class="flex items-center gap-4 ">
                            <div class="text-right">
                                <h1 class="font-bold text-xl">M. John Doe</h1>
                                <h2>Vice-Principal</h2>
                            </div>
                            <div class="h-[50px] w-[50px] rounded-full border">
                                <img src="/images/profile.jpg" alt="" class="w-full h-full rounded-full">
                            </div>
                        </div>
                    </div>
                </div>
                <div class="w-full h-[calc(100%-50px)] overflow-y-scroll custom-nav-hidden">
                    <div class="w-full">
                        
                        <div class="w-full">
                            <div>
                                <div class="text-2xl font-bold flex items-center gap-4">
                                    <h1>Form 5 A</h1>
                                    <h1>2nd Term</h1>
                                </div>
                            </div>
                        </div>
                        <section class="w-full py-3">
                            <div class="w-full border border-[#007194] h-[250px] rounded-xl flex flex-col justify-between items-start">
                                <div class="w-full h-[60px] border-b border-[#007194] flex">
                                    <div class="w-[35%] flex items-center justify-between px-2">
                                        <h1>Class Summary</h1>
                                        <div class="text-2xl font-bold flex items-center gap-4">
                                            <h1>Form 5 A</h1>
                                            <h1>2nd Term</h1>
                                        </div>
                                    </div>
                                </div>
                                <div class="w-full flex items-center justify-between">
                                    <div class="h-full w-[25%] flex justify-center items-center gap-4">
                                        <font-awesome-icon icon="fa-solid fa-users" class="fa-2x"/>
                                        <div class="flex flex-col justify-center items-center">
                                            <span class="font-extrabold text-5xl">80</span>
                                            <span class="font-extrabold text-xl">Students</span>
                                        </div>
                                    </div>
                                    <div class="flex gap-3 w-[75%]">
                                        <LevelStat title="Median" :increased="true">
                                            <div class="py-2 flex items-center gap-2">
                                                <span class="text-[#FFA800]">
                                                    <font-awesome-icon icon="fa-solid fa-code-fork" class="fa-1x"/>
                                                </span>
                                                <span class="font-extrabold text-2xl">38/50</span>
                                            </div>
                                        </LevelStat>
                                        <LevelStat title="Highest Mark" :increased="true">
                                            <div class="py-2 flex items-center gap-2">
                                                <span class="text-[#1CB647] border border-[#1CB647] rounded-full h-[30px] w-[30px] flex justify-center items-center">
                                                    <font-awesome-icon icon="fa-solid fa-chevron-up" class="fa-1x"/>
                                                </span>
                                                <span class="font-extrabold text-2xl">48/50</span>
                                            </div>
                                        </LevelStat>
                                        <LevelStat title="Lowest Mark" :increased="true" >
                                            <div class="py-2 flex items-center gap-2">
                                                <span class="text-[#FF6B6B] border border-[#FF6B6B] rounded-full h-[30px] w-[30px] flex justify-center items-center">
                                                    <font-awesome-icon icon="fa-solid fa-chevron-down" class="fa-1x"/>
                                                </span>
                                                <span class="font-extrabold text-2xl">18/50</span>
                                            </div>
                                        </LevelStat>
                                        <LevelStat title="Underperformers" :increased="false" >
                                            <div class="py-2 flex items-center gap-2">
                                                <span class="text-[#FF6B6B] border border-[#FF6B6B] rounded-full h-[30px] w-[30px] flex justify-center items-center">
                                                    <font-awesome-icon icon="fa-solid fa-graduation-cap" class="fa-1x"/>
                                                </span>
                                                <span class="font-extrabold text-2xl">28/50</span>
                                            </div>
                                        </LevelStat>
                                    </div>
                                    <div></div>
                                </div>
                                <div class="w-full h-[60px] border-t border-[#007194] py-2 flex justify-center items-center">
                                    <nuxt-link to="/" class="text-white px-12 bg-[#007194] py-2 rounded-md text-lg font-bold">
                                        View complete repport
                                    </nuxt-link>
                                </div>
                            </div>
                        </section>
                    </div>
                    <div class="my-2">
                        <slot />
                    </div>
                    <div class="w-full flex justify-between items-center">
                        <div class="w-[75%] h-[230px] border border-[#00A7DA] rounded-lg flex justify-between items-center px-2">
                            <div class="h-full w-[80%]">
                                <div class="w-full flex flex-col justify-between items-start h-full py-2">
                                    <div class="w-full">
                                        <h1>Send Message to Teacher(s)</h1>
                                        <div class="flex justify-end items-center gap-4">
                                            <select name="" id="" class="px-8 py-1 text-left border border-[#00A7DA] rounded-lg">
                                                <option value="">Pick a subject</option>
                                                <option value="">subject 1</option>
                                            </select>
                                            <select name="" id="" class="px-8 py-1 text-left border border-[#00A7DA] rounded-lg">
                                                <option value="">Pick a subject</option>
                                                <option value="">subject 1</option>
                                            </select>
                                        </div>
                                    </div>
                                    <div class="w-full h-[150px] bg-[#9CC3D3] border rounded-lg border-[#00A7DA]">
                                        <Textarea class="h-full w-full rounded-lg p-2"></Textarea>
                                    </div>
                                </div>
                            </div>
                            <div class="h-full w-[20%] flex flex-col justify-between items-center py-10 gap-4">
                                <div class="flex flex-col">
                                    <span class="space-x-2">
                                        <input type="radio" name="" id="primary">
                                        <label for="primary">Primary</label>
                                    </span>
                                    <span class="space-x-2">
                                        <input type="radio" name="" id="secondary">
                                        <label for="secondary">Secondary</label>
                                    </span>
                                </div>
                                <button class="border border-[#00A7DA] bg-[#00A7DA] px-8 rounded-lg py-1 text-white space-x-3">
                                    <span>send</span>
                                    <font-awesome-icon icon="fa-solid fa-paper-plane" class="fa-1x"/>
                                </button>
                            </div>
                        </div>
                    </div>
                </div>
            </div>
            <div class="w-full h-[50px] flex justify-center items-center font-bold">
                <p>Copyright &copy; TEFA {{ new Date().getFullYear() }}</p>
            </div>
        </div>
        <div class="absolute bottom-2 right-2 h-[80px] w-[80px] border-2 border-[#007194] text-[#007194] rounded-full flex flex-col justify-center items-center">
            <span class="font-bold">TEFA</span>
            <span class="font-bold">Afrik</span>
        </div>
    </div>
</template>

<script lang="ts" setup>
import { ref } from "vue"
const fakeText = ref("Lorem ipsum dolor sit amet consectetur adipisicing elit. Placeat, et. Repellendus a voluptas, ab quos perspiciatis voluptate recusandae nihil provident et fugiat autem debitis molestias modi, similique rerum maxime amet.")
</script>

<style lang="scss" scoped>


</style>