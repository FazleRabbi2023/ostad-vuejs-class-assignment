<script setup>
import { ref, reactive } from 'vue'


const lampBtn = reactive({
    activeState: [false, false, false],
    activeText: ['on', 'on', 'on'],
    activeClass: new Array(3).fill('bg-gray-500 hover:bg-gray-700 text-orange-500')
})

function operation(index) {
    lampBtn.activeState[index] = !lampBtn.activeState[index];
    lampBtn.activeText[index] = lampBtn.activeState[index] == true ? 'off' : 'on';
    lampBtn.activeClass[index] = lampBtn.activeState[index] == true ? 'bg-blue-500 hover:bg-blue-700 text-white' : 'bg-gray-500 hover:bg-gray-700 text-orange-500';
}

</script>

<template>
  <section class="container mx-auto flex items-center flex-col">
        <h1 class="text-center text-2xl py-10">Assignment</h1>
        <p class="p-5">Make These Buttons Work</p>
        <div class="flex justify-between space-x-6">
            <div class="p-10 border w-96 flex flex-col space-y-16">
                <button @click="operation(0)" :class="lampBtn.activeClass[0]" class="font-bold py-2 px-4 rounded">
                    Turn Light 1 {{lampBtn.activeText[0]}}
                </button>
                <button @click="operation(1)" :class="lampBtn.activeClass[1]" class="font-bold py-2 px-4 rounded">
                    Turn Light 2 {{lampBtn.activeText[1]}}
                </button>
                <button @click="operation(2)" :class="lampBtn.activeClass[2]" class="font-bold py-2 px-4 rounded">
                    Turn Light 3 {{lampBtn.activeText[2]}}
                </button>
            </div>
            <div class="py-6 px-6 border w-50 flex flex-col space-y-6">
                <img class="w-20" :src="true==lampBtn.activeState[0]?'//img.icons8.com/?size=512&id=12244&format=png':'//img.icons8.com/?size=512&id=75&format=png'" alt="">
                <img class="w-20" :src="true==lampBtn.activeState[1]?'//img.icons8.com/?size=512&id=12244&format=png':'//img.icons8.com/?size=512&id=75&format=png'" alt="">
                <img class="w-20" :src="true==lampBtn.activeState[2]?'//img.icons8.com/?size=512&id=12244&format=png':'//img.icons8.com/?size=512&id=75&format=png'" alt="">
            </div>
        </div>
    </section>
</template>

<style scoped></style>