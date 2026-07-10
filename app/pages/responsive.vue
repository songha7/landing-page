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

        alert(`Name: ${name.value}\nEmail: ${email.value}`)
    }

}



</script>

<template>
    <div class="flex relative">
        <div class="mx-4">
            <div class="w-1/2 flex items-start justify-start h-64">
                <div class="flex flex-col z-10">
                    <p class="text-white
                    font-bold
                    text-2xl">Ricky
                    </p>
                    <span class="
                    text-white
                    text-sm 
                    font-extralight 
                    tracking-[0.5rem]">CYCLES
                    </span>
                    <p class="font-extrabold text-white italic pt-10 pl-6">
                        Get 70% Off Bikes for Commuters
                    </p>
                    <button @click="scrollToForm" class="bg-white ml-5 mt-6">BUY IT</button>
                </div>
            </div>
            <div class="w-1/2 justify-end">
                <img src="/images/bike1.png" alt="bike" class="scale-x-[-1] object-contain
                absolute inset-10">
            </div>
        </div>
    </div>
    <div class="flex items-center">
        <div class=" text-center m-6">
            <p class="items-center justify-center flex flex-row text-black ">
                <h1 class="text-3xl md:text-5xl font-bold">DEAL OF THE WEEK</h1>
                <h2 class="text-xl font-mono md:text-red-500 pb-10 ">Pardus Robin Series</h2>
                <h3 class="text-sm font-sans ">Pardus is the official bicycle supplier of the Chinese National Cycling Team and is backed by the Taishan Sports Industry Group, which has provided equipment for the Olympic Games for over 40 years.</h3>
            </p>
        </div>
    </div>
    <div ref="formSection" class=" items-center justify-center rounded-xl m-10">
        <h2 class="text-xl text-center font-semibold text-gray-800">FILL OUT THE FORM</h2>
        <form @submit.prevent="handleSubmit">
            <label class="text-gray-500 pb-1 pt-3 text-sm mt-5">NAME</label>
            <input v-model="name" type="text" class="border-b border-gray-400 outline-none bg-transparent w-full pb-0.2"/>
            <label class="text-gray-500 pb-1 pt-3 text-sm mt-2">EMAIL</label>
            <input v-model="email" type="text" class="border-b border-gray-400 outline-none bg-transparent w-full pb-0.2"/>
            <button type="submit" class="border-black cursor-pointer bg-[#1d1d1b] text-2xl text-white rounded-2xl w-full mt-10 pt-3 pr-5 pl-5 pb-3 ">Buy it</button>
        </form>
    </div>
    <div class="max-w-5xl mx-auto flex flex-col gap-12 ">
        <h2 class="text-4xl font-medium text-center uppercase tracking-wide">
            BEST QUALITY
        </h2>
        <div class="grid grid-cols-1 md:grid-cols-3 gap-8 m-5 text-center">
            <div class="flex flex-col bg-white gap-4">
            <div class="bg-[#fef1d6] aspect-full w-full overflow-hidden flex items-center justify-center rounded-xl">
                <img src="/images/bikethak.png" alt="Lightweight Design" class="w-full h-full object-cover scale-x-[-1]"/>
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
            <img src="/images/bikekeb.png" alt="Comfortable Ergonomics" class="w-full h-full object-cover scale-x-[-1]" />
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
            <img src="/images/bikehandbar.png" alt="Practical Accessories" class="w-full h-full object-cover scale-x-[-1]" />
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