<script setup lang="ts">
import { ref } from "vue";
import { mnozymy, multiVal } from "../models";
import MultiButton from "./MultiButton.vue";

let zero = ref();
let one = ref();
let two = ref();
let three = ref();
let four = ref();
let five = ref();
let six = ref();
let seven = ref();
let eight = ref();
let nine = ref();
let ten = ref();

let spr0 = ref();
let spr1 = ref();
let spr2 = ref();
let spr3 = ref();
let spr4 = ref();
let spr5 = ref();
let spr6 = ref();
let spr7 = ref();
let spr8 = ref();
let spr9 = ref();
let spr10 = ref();

//defineProps<{ msg: string }>();

const resTab = () => {
  if (zero.value !== mnozymy.threeZero) {
    spr0.value = multiVal.sad;
  }
  if (mnozymy.threeZero == zero.value) {
    spr0.value = multiVal.smiling;
  }
  if (!zero.value) {
    spr0.value = multiVal.warring;
  }
  //przez jeden
  if (one.value !== mnozymy.threeOne) {
    spr1.value = multiVal.sad;
  }
  if (mnozymy.threeOne == one.value) {
    spr1.value = multiVal.smiling;
  }
  if (!one.value) {
    spr1.value = multiVal.warring;
  }
  //przez dwa
  if (three.value !== mnozymy.threeThree) {
    spr2.value = multiVal.sad;
  }
  if (mnozymy.threeThree == three.value) {
    spr2.value = multiVal.smiling;
  }
  if (!one.value) {
    spr2.value = multiVal.warring;
  }
  //przez 3
  if (three.value !== mnozymy.threeThree) {
    spr3.value = multiVal.sad;
  }
  if (mnozymy.threeThree == three.value) {
    spr3.value = multiVal.smiling;
  }
  if (!three.value) {
    spr3.value = multiVal.warring;
  }
  //przez 4
  if (four.value !== mnozymy.threeFour) {
    spr4.value = multiVal.sad;
  }
  if (mnozymy.threeFour == four.value) {
    spr4.value = multiVal.smiling;
  }
  if (!four.value) {
    spr4.value = multiVal.warring;
  }
  //przez 5
  if (five.value !== mnozymy.threeFive) {
    spr5.value = multiVal.sad;
  }
  if (mnozymy.threeFive == five.value) {
    spr5.value = multiVal.smiling;
  }
  if (!five.value) {
    spr5.value = multiVal.warring;
  }
  //przez 6
  if (six.value !== mnozymy.threeSix) {
    spr6.value = multiVal.sad;
  }
  if (mnozymy.threeSix == six.value) {
    spr6.value = multiVal.smiling;
  }
  if (!six.value) {
    spr6.value = multiVal.warring;
  }
  //przez 7
  if (seven.value !== mnozymy.threeSeven) {
    spr7.value = multiVal.sad;
  }
  if (mnozymy.threeSeven == seven.value) {
    spr7.value = multiVal.smiling;
  }
  if (!seven.value) {
    spr7.value = multiVal.warring;
  }
  //przez 8
  if (eight.value !== mnozymy.threeEight) {
    spr8.value = multiVal.sad;
  }
  if (mnozymy.threeEight == eight.value) {
    spr8.value = multiVal.smiling;
  }
  if (!eight.value) {
    spr8.value = multiVal.warring;
  }
  //przez 9
  if (nine.value !== mnozymy.threeNine) {
    spr9.value = multiVal.sad;
  }
  if (mnozymy.threeNine == nine.value) {
    spr9.value = multiVal.smiling;
  }
  if (!nine.value) {
    spr9.value = multiVal.warring;
  }
  //przez 10
  if (ten.value !== mnozymy.threeTen) {
    spr10.value = multiVal.sad;
  }
  if (mnozymy.threeTen == ten.value) {
    spr10.value = multiVal.smiling;
  }
  if (!ten.value) {
    spr10.value = multiVal.warring;
  }
};

const resets = () => {
  zero.value = "";
  one.value = "";
  two.value = "";
  three.value = "";
  four.value = "";
  five.value = "";
  six.value = "";
  seven.value = "";
  eight.value = "";
  nine.value = "";
  ten.value = "";
  spr0.value = "";
  spr1.value = "";
  spr2.value = "";
  spr3.value = "";
  spr4.value = "";
  spr5.value = "";
  spr6.value = "";
  spr7.value = "";
  spr8.value = "";
  spr9.value = "";
  spr10.value = "";
};
</script>

<template>
  <div
    class="component-rule bg-gradient-to-r from-orange-400 to-orange-500 p-2"
  >
    <div class="flex mb-2 gap-2 items-center justify-center">
      <div class="">3x0 =</div>
      <div>
        <input
          type="text"
          class="input-text"
          v-model="zero"
          :maxlength="multiVal.maxlen"
        />
      </div>
      <div class="material-symbols-outlined absolute ml-[136px]">
        {{ spr0 }}
      </div>
    </div>

    <div class="flex mb-2 gap-2 items-center justify-center">
      3x1 =
      <div>
        <input
          type="text"
          class="input-text"
          v-model="one"
          :maxlength="multiVal.maxlen"
        />
      </div>
      <div class="material-symbols-outlined absolute ml-[136px]">
        {{ spr1 }}
      </div>
    </div>
    <div class="flex mb-2 gap-2 items-center justify-center">
      3x2 =
      <div>
        <input
          type="text"
          class="input-text"
          v-model="two"
          :maxlength="multiVal.maxlen"
        />
      </div>
      <div class="material-symbols-outlined absolute ml-[136px]">
        {{ spr2 }}
      </div>
    </div>
    <div class="flex mb-2 gap-2 items-center justify-center">
      3x3 =
      <div>
        <input
          type="text"
          class="input-text"
          v-model="three"
          :maxlength="multiVal.maxlen"
        />
      </div>
      <div class="material-symbols-outlined absolute ml-[136px]">
        {{ spr3 }}
      </div>
    </div>
    <div class="flex mb-2 gap-2 items-center justify-center">
      3x4 =
      <div>
        <input
          type="text"
          class="input-text"
          v-model="four"
          :maxlength="multiVal.maxlen"
        />
      </div>
      <div class="material-symbols-outlined absolute ml-[136px]">
        {{ spr4 }}
      </div>
    </div>
    <div class="flex mb-2 gap-2 items-center justify-center">
      3x5 =
      <div>
        <input
          type="text"
          class="input-text"
          v-model="five"
          :maxlength="multiVal.maxlen"
        />
      </div>
      <div class="material-symbols-outlined absolute ml-[136px]">
        {{ spr5 }}
      </div>
    </div>
    <div class="flex mb-2 gap-2 items-center justify-center">
      3x6 =
      <div>
        <input
          type="text"
          class="input-text"
          v-model="six"
          :maxlength="multiVal.maxlen"
        />
      </div>
      <div class="material-symbols-outlined absolute ml-[136px]">
        {{ spr6 }}
      </div>
    </div>
    <div class="flex mb-2 gap-2 items-center justify-center">
      3x7 =
      <div>
        <input
          type="text"
          class="input-text"
          v-model="seven"
          :maxlength="multiVal.maxlen"
        />
      </div>
      <div class="material-symbols-outlined absolute ml-[136px]">
        {{ spr7 }}
      </div>
    </div>
    <div class="flex mb-2 gap-2 items-center justify-center">
      3x8 =
      <div>
        <input
          type="text"
          class="input-text"
          v-model="eight"
          :maxlength="multiVal.maxlen"
        />
      </div>
      <div class="material-symbols-outlined absolute ml-[136px]">
        {{ spr8 }}
      </div>
    </div>
    <div class="flex mb-2 gap-2 items-center justify-center">
      3x9 =
      <div>
        <input
          type="text"
          class="input-text"
          v-model="nine"
          :maxlength="multiVal.maxlen"
        />
      </div>
      <div class="material-symbols-outlined absolute ml-[136px]">
        {{ spr9 }}
      </div>
    </div>
    <div class="flex mb-2 gap-2 items-center justify-center">
      3x10 =
      <div class="mr-2">
        <input
          type="text"
          class="input-text"
          v-model="ten"
          :maxlength="multiVal.maxlen"
        />
      </div>
      <div class="material-symbols-outlined absolute ml-[136px]">
        {{ spr10 }}
      </div>
    </div>
    <div class="flex justify-center flex-row">
      <MultiButton @check="resTab()" @reset="resets()"></MultiButton>
    </div>
  </div>
</template>
