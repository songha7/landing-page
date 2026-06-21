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
    <section class="bg-cyan-300 px-6 py-16 md:py-20">
      <div class="max-w-5xl mx-auto flex flex-col md:flex-row items-center gap-10">
        <div class="w-full md:w-1/2">
          <p class="text-white
            font-bold
            text-3xl
            leading-tight">
            RICKY 
            <span class="block
            text-sm
            font-normal
            tracking-[0.5em]">CYCLES</span>
          </p>
          <h1 class="text-white font-extrabold text-2xl md:text-5xl leading-tight mt-6 mb-8">
            Get 70% Off Bikes<br />for Commuters
          </h1>
          <Button class="bg-white text-2xl text-black hover:bg-neutral-100 font-bold uppercase tracking-wide px-20 py-5">
            Buy it
          </Button>
        </div>
        <div class="w-full md:w-1/2 flex justify-center md:justify-end mt-0 md:mt-0">
          <img src="/images/bike1.png" alt="Ricky Cycles commuter road bike" class="w-full max-w-400 object-contain scale-x-[-1]" />
        </div>
      </div>
    </section>
    <section class="bg-red-400 px-6 py-16 md:py-20">
      <p class="max-w-5xl mx-auto  text-black ">
        <h1 class="text-5xl md:text-6xl font-extrabold">DEAL OF THE WEEK</h1>
        <h2 class="text-4xl md:text-5xl font-mono ">Pardus Robin Series</h2>
        <h3 class="text-xl md:text-l font-sans">Pardus is the official bicycle supplier<br /> of the Chinese National Cycling Team <br />and is backed by the Taishan Sports <br />Industry Group, which has provided<br /> equipment for the Olympic Games for over 40 years.</h3>
      </p>
    </section>
<section class="bg-green-500 text-black px-6 py-16 md:py-24">
  <div class="max-w-5xl mx-auto flex flex-col gap-12">
    <h2 class="text-2xl md:text-3xl font-extrabold text-center uppercase tracking-wide">
      BEST QUALITY
    </h2>
    <div class="grid grid-cols-1 md:grid-cols-3 gap-8">
      <div class="flex flex-col bg-white gap-4">
        <div class="bg-[#ecc65c] aspect-full w-full overflow-hidden flex items-center justify-center">
          <img src="/images/bikethak.PNG" alt="Lightweight Design" class="w-full h-full object-cover"/>
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
        <div class="bg-[#da91f0] aspect-full w-full overflow-hidden flex items-center justify-center">
          <img src="/images/bikekeb.PNG" alt="Comfortable Ergonomics" class="w-full h-full object-cover" />
        </div>
        <!-- Content text -->
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
        <div class="bg-[#41f1c8] aspect-full w-full overflow-hidden flex items-center justify-center">
          <img src="/images/bikehandbar.PNG" alt="Practical Accessories" class="w-full h-full object-cover" />
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