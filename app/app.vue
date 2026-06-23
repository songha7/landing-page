<script setup lang="ts">
useHead({ title: 'Ricky Cycles' })

import {
  Form,
  FormControl,
  FormDescription,
  FormField,
  FormItem,
  FormLabel,
  FormMessage,
} from '@/components/ui/form'
</script>
<template>
    <section class="bg-[#1ec7b8] ">
      <div class="max-w-5xl mx-auto flex md:flex-row items-center gap-10">
        <div class="w-full pb-15 md:w-1/2">
          <p class="text-white
            font-bold
            text-3xl
            pt-7
            leading-tight">
            RICKY 
            <span class="block
            text-sm
            font-normal
            tracking-[0.5em]">CYCLES</span>
          </p>
          <h1 class="text-white font-extrabold text-2xl md:text-5xl leading-tight mt-10 mb-8">
            Get 70% Off Bikes<br />for Commuters
          </h1>
          <Button class="bg-white text-2xl text-black hover:bg-neutral-100 font-bold tracking-wide rounded-lg px-20 py-4 ">
            BUY IT
          </Button>
        </div>
        <div class="min-w-0 md:w-1/2 flex justify-end padding:0 md:justify-end">
          <img src="/images/bike1.png" alt="Ricky Cycles commuter road bike" class="w-full max-w-400 object-contain scale-x-[-1]" />
        </div>
      </div>
    </section>
    <section class="bg-green-400 flew flew-row">
      <div class="w-1/2 flex flex-col items-center gap-10" >
          <p class="max-w-5xl mx-auto flex flex-col text-black ">
            <h1 class="text-4xl font-extrabold">DEAL OF THE WEEK</h1>
            <h2 class="text-3xl font-mono pb-10 ">Pardus Robin Series</h2>
            <h3 class="text-xl font-sans">Pardus is the official bicycle supplier<br /> of the Chinese National Cycling Team <br />and is backed by the Taishan Sports <br />Industry Group, which has provided<br /> equipment for the Olympic Games for over 40 years.</h3>
          </p>
      </div>
      <div class=" w-1/2 bg-amber-800 justify-end ">
        fill
      </div>  
    </section>
    <section class="bg-white text-black py-8">
      <div class="max-w-5xl mx-auto flex flex-col gap-12">
        <h2 class="text-6xl font-medium text-center uppercase tracking-wide">
          BEST QUALITY
        </h2>
        <div class="grid grid-cols-1 md:grid-cols-3 gap-8">
          <div class="flex flex-col bg-white gap-4">
            <div class="bg-[#fef1d6] aspect-full w-full overflow-hidden flex items-center justify-center">
              <img src="/images/bikethak.PNG" alt="Lightweight Design" class="w-full h-full object-cover scale-x-[-1]"/>
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
            <div class="bg-[#d0d0ee] aspect-full w-full overflow-hidden flex items-center justify-center">
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
            <div class="bg-[#b5e5df] aspect-full w-full overflow-hidden flex items-center justify-center ">
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
    </section>
</template>
<style scoped>

</style>