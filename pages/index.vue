<template>
    <div class="w-full h-full flex justify-between items-center">
      <div class="h-full w-full md:w-[20%] overflow-hidden text-[#00A7DA]">
        <LeftLibrary />
      </div>
      <div class="h-full w-full md:w-[60%] md:overflow-hidden">
        <div class="flex justify-center items-start w-full overflow-x-hidden h-full overflow-y-scroll px-8">
          <div class="grid grid-cols-2 gap-8 w-full py-5">
            <SubjectCard v-for="subject in subjects" :key="subject.title" :subject="subject"/>
            
          </div>
        </div>
      </div>
      <div class="h-full w-full md:w-[20%] overflow-hidden text-[#00A7DA] relative">
        <div class="absolute bottom-0  right-0 p-4">
          <p>copyright &copy; TEFA {{ new Date().getFullYear() }}</p> 
        </div>
        <div class="w-full h-full flex justify-center items-center px-8">
          <div class="flex flex-col justify-center items-center w-full gap-4">
            <div class="w-full flex flex-col justify-center items-center gap-4">
              <p class="font-bold">0 Days left</p>
              <ProgressBar foreground="bg-orange-800" background="bg-orange-50" fill="w-[2%]"/>
            </div>
            <div class="w-full flex flex-col justify-center items-center mt-4">
              <div class="w-[90px] h-[90px] border"></div>
              <div class="bg-orange-600 w-[45%] h-[2px] rounded-[10px] mt-2" />
              <p class="font-bold mt-2">Monthly Payment</p>
            </div>
            <div class="flex flex-col text-lg">
              <p>Gives acces to all Subjects</p>
              <p class="text-[#E28305]">5 000 Fcfa for November</p>
              
            </div>
            <div>
              <nuxt-link to="/payment" class="py-2 px-4 bg-red-600 rounded-[25px] text-2xl text-white font-bold flex items-center gap-3">
                <span>Pay Now</span>
                <span>>></span>
              </nuxt-link>
            </div>
            <div>
              <nuxt-link to="/about-payments" class="flex items-center gap-2">
                <span>?</span> 
                <span>About payments</span>
              </nuxt-link>
            </div>
          </div>
        </div>
      </div>
    </div>
</template>

<script setup lang="ts">
import { ref } from "vue"
const subjects = ref([
  {
    title: "Computer Science",
    image: '/icons/Computer_Science_Icon_1.png',
    teacher: "Teacher's name",
    studentRank: 50,
    presentStudents: 80,
    allStudents: 80,
    progress: 20,
    evaluation: 5,
  },
  {
    title: "Pure Mathematics With Statistics",
    image: '/icons/Statistics_Icon_2.png',
    teacher: "Teacher's name",
    studentRank: 50,
    presentStudents: 80,
    allStudents: 80,
    progress: 20,
    evaluation: 5,
  },
  {
    title: "Economy",
    image: '/icons/Economics_Icon_4.png',
    teacher: "Teacher's name",
    studentRank: 50,
    presentStudents: 80,
    allStudents: 80,
    progress: 20,
    evaluation: 5,
  },
  {
    title: "Chemistry",
    image: '/icons/Chemistry_Icon_1.png',
    teacher: "Teacher's name",
    studentRank: 50,
    presentStudents: 80,
    allStudents: 80,
    progress: 20,
    evaluation: 5,
  },
  {
    title: "English",
    image: '/icons/Language_Icon_1.png',
    teacher: "Teacher's name",
    studentRank: 50,
    presentStudents: 80,
    allStudents: 80,
    progress: 20,
    evaluation: 5,
  },
  {
    title: "Biology",
    image: '/icons/Biology_Icon_1.png',
    teacher: "Teacher's name",
    studentRank: 50,
    presentStudents: 80,
    allStudents: 80,
    progress: 20,
    evaluation: 5,
  },
])
</script>

<style scoped>


</style>