<script setup lang="ts">
import { buttonName } from "../models";

const emit = defineEmits(["check", "reset"]);
</script>

<template>
  <div class="max-md:w-auto flex mt-1">
    <button
    @click="$emit('check')"
    class="btn bg-red-600 text-sm hover:bg-gray-500 "
    >
    {{ buttonName.btnCheck }}
  </button>
  <button
    @click="$emit('reset')"
    class="btn bg-black text-sm font-mono hover:bg-gray-500 "
    >
    {{ buttonName.btnReset }}
  </button>
</div>
</template>

<style></style>
