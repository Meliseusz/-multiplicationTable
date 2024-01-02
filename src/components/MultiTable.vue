<script setup lang="ts">
import MultiTabZero from "./MultiTabZero.vue";
import MultiTabOne from "./MultiTabOne.vue";
import MultiTabTwo from "./MultiTabTwo.vue";
import MultiTabThree from "./MultiTabThree.vue";
import MultiTabFour from "./MultiTabFour.vue";
import MultiTabFive from "./MultiTabFive.vue";
import MultiTabSix from "./MultiTabSix.vue";
import MultiTabSeven from "./MultiTabSeven.vue";
import MultiTabEight from "./MultiTabEight.vue";
import MultiTabNine from "./MultiTabNine.vue";
import MultiTabTen from "./MultiTabTen.vue";

import { multiVal } from "../models";

let IPyear = new Date().getFullYear();
</script>

<template>
 <div class=" flex flex-col">

   <div
   class="flex justify-center max-md:w-[336px] rounded mt-5 bg-slate-800 w-full mx-auto max-w-screen-xl p-1 "
   >
   <h1 class="text-white font-mono md:text-4xl text-2xl ">
      {{ multiVal.nameApp }}
    </h1>
  </div>

  <div class="flex flex-col p-2 text-blue-800 rounded">
    <div class="md:flex md:flex-row justify-center">
      <div class="p-1">
        <MultiTabZero />
      </div>
      <div class="p-1">
        <MultiTabOne />
      </div>
      <div class="p-1">
        <MultiTabTwo />
      </div>

      <div class="p-1">
        <MultiTabThree />
      </div>
    </div>
    
    <div class="md:flex md:flex-row justify-center">
      <div class="p-1">
        <MultiTabFour />
      </div>

      <div class="p-1">
        <MultiTabFive />
      </div>
      <div class="p-1">
        <MultiTabSix />
      </div>
      <div class="p-1">
        <MultiTabSeven />
      </div>
    </div>
    <div class="md:flex md:flex-row justify-center">
      <div class="p-1">
        <MultiTabEight />
      </div>
      <div class="p-1">
        <MultiTabNine />
      </div>
      <div class="p-1">
        <MultiTabTen />
      </div>
    </div>
    <footer
      class="bg-gradient-to-r from-slate-500 to-slate-800 rounded-lg shadow m-1 dark:bg-gray-800"
    >
      <div class="w-full mx-auto max-w-screen-xl p-1 text-right">
        <div class="text-sm text-white dark:text-gray-400 text-right">
          © {{ IPyear }}
          <a href="https://diseno-art.pl/" class="hover:underline">{{
            multiVal.companyName
          }}</a
          >.
          <div class="text-right">
            All Rights Reserved. Ver. {{ multiVal.version }}
          </div>
        </div>
      </div>
    </footer>
  </div>
</div>
</template>

<style scoped>

</style>
