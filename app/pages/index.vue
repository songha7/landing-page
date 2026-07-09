<script setup lang="ts">
import { ref } from 'vue'
// function alertMsg() {
//     alert('oasidjoij')
// }
// @click="alertMsg"
const name = ref('')
const email = ref('')
const formSection = ref<HTMLElement | null>(null)

function scrollToForm() {
    formSection.value?.scrollIntoView({ behavior: 'smooth', block: 'start' })
}

function handleSubmit() {
    if (!name.value.trim() || !email.value.trim()) {
        alert('please fill both Name and Email.')
    } else {   

    }
    alert('Name: ${name.value}\nEmail: ${email.value}')

}



</script>

<template>
    <div class="bg-[#1ec7b8] flex relative h-64 md:h-110 overflow-hidden">
        <div class="pr-20 mx-10 flex flex-col md:flex-row">
            <div class="w-1/2 flex items-start justify-start ">
                <div class="flex flex-col md:px-20 md:pt-10 z-10">
                    <p class="text-white
                    font-bold
                    text-2xl
                    md:text-3xl
                    uppercase">Ricky
                    </p>
                    <span class="
                    text-white
                    text-sm 
                    font-extralight 
                    tracking-[0.5rem]">CYCLES
                    </span>
                    <p class="font-extrabold text-white italic md:text-5xl pt-10 pl-6 ">
                        Get 70% Off Bikes for Commuters
                    </p>
                    <button @click="scrollToForm" class="bg-white ml-5 mt-6 md:mt-10 md:py-5 rounded-2xl md:text-3xl">BUY IT</button>
                </div>
            </div>
            <div class="w-1/2 justify-end">
                <img src="/images/bike1.PNG" alt="bike" class="scale-x-[-1] object-contain w-auto h-72 md:h-auto md:w-2xl
                absolute bottom-0 right-0">
            </div>
        </div>
    </div>
    <div class="flex flex-col md:flex-row">
        <div class="flex md:w-1/2 items-center">
            <div class=" text-center m-6 md:mx-23">
                <p class="items-center justify-center flex flex-row text-black ">
                    <h1 class="text-3xl md:text-5xl font-bold md:pb-2">DEAL OF THE WEEK</h1>
                    <h2 class="text-xl md:text-3xl font-mono pb-10 ">Pardus Robin Series</h2>
                    <h3 class="text-sm md:text-lg font-sans ">Pardus is the official bicycle supplier of the Chinese National Cycling Team and is backed by the Taishan Sports Industry Group, which has provided equipment for the Olympic Games for over 40 years.</h3>
                </p>
            </div>
        </div>
        <div class="md:w-1/2 md:relative ">
            <div class="md:absolute md:left-25 md:-top-25">
                <div ref="formSection" class="md:bg-white py-5 px-10  shadow-2xl md:w-1/2 items-center justify-center rounded-xl m-10">
                    <h2 class="text-xl md:text-2xl text-center mb-6 font-semibold text-gray-800">FILL OUT THE FORM</h2>
                    <form @submit.prevent="handleSubmit" class="space-y-8">
                        <label class="text-gray-500 pb-1  text-sm mt-5">NAME</label>
                        <input v-model="name" type="text" class="border-b border-gray-400 outline-none bg-transparent w-full pb-0.2"/>
                        <label class="text-gray-500 pb-1 pt-3 text-sm mt-2">EMAIL</label>
                        <input v-model="email" type="text" class="border-b border-gray-400 outline-none bg-transparent w-full pb-0.2"/>
                        <button type="submit" class="border-black bg-[#1d1d1b] text-2xl text-white rounded-2xl w-full mt-10 pt-3 pr-5 pl-5 pb-3 ">Buy it</button>
                    </form>
                </div>
            </div>
        </div>
    </div>
    <div class="max-w-5xl mx-auto flex flex-col gap-12 ">
        <h2 class="text-4xl font-medium text-center uppercase tracking-wide">
            BEST QUALITY
        </h2>
        <div class="grid grid-cols-1 md:grid-cols-3 gap-8 m-5 text-center">
            <div class="flex flex-col bg-white gap-4">
            <div class="bg-[#fef1d6] aspect-full w-full overflow-hidden flex items-center justify-center rounded-xl"><img src="/images/bikethak.PNG" alt="Lightweight Design" class="w-full h-full object-cover scale-x-[-1]"/>
            </div>
            <div class="flex flex-col gap-2">
                <h3 class="font-extrabold text-base uppercase tracking-tight leading-tight">
                LIGHTWEIGHT DESIGN:
                </h3>
                <p class="text-neutral-600 text-sm ">
                Built with an advanced ultra-lightweight EPS+ Carbon Frame to shred weight without losing structural strength.
                </p>
            </div>
            </div>
            <div class=" bg-white flex flex-col gap-4">
            <!-- Crop image container -->
            <div class="bg-[#d0d0ee] aspect-full w-full overflow-hidden flex items-center justify-center rounded-xl">
            <img src="/images/bikekeb.PNG" alt="Comfortable Ergonomics" class="w-full h-full object-cover scale-x-[-1]" />
            </div>
            <div class="flex flex-col gap-2">
            <h3 class="font-extrabold text-base uppercase tracking-tight leading-tight">
                COMFORTABLE ERGONOMICS:
            </h3>
            <p class="text-neutral-600 text-sm leading-relaxed">
                Balanced endurance geometry frame keeps you in an optimal, fatigue-free position on your long daily commutes.
            </p>
            </div>
        </div>
        <div class="bg-white flex flex-col gap-4">
            <!-- Crop image container -->
            <div class="bg-[#b5e5df] aspect-full w-full overflow-hidden flex items-center justify-center rounded-xl">
            <img src="/images/bikehandbar.PNG" alt="Practical Accessories" class="w-full h-full object-cover scale-x-[-1]" />
            </div>
            <!-- Content text -->
            <div class="flex flex-col gap-2">
            <h3 class="font-extrabold text-base uppercase tracking-tight leading-tight">
                PRACTICAL ACCESSORIES:
            </h3>
            <p class="text-neutral-600 text-sm leading-relaxed">
                Equipped with premium all-weather disc brakes for instant stopping power, alongside speed-sustaining deep-section MVMT carbon wheels.
            </p>
            </div>
        </div>
        </div>
    </div>

</template>

<style scoped></style>