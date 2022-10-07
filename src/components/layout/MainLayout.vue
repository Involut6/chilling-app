<script setup>
import SideBar from "../SideBar.vue";
import ChevronDownIcon from "../icons/ChevronDownIcon.vue";
import { ref } from "vue";

const dropDown = ref(false);
function toggleDropDown() {
    dropDown.value = !dropDown.value;
}
</script>

<template>
  <div class="overflow-y-auto flex h-[100vh] bg-[#F1F5F9]">
    <SideBar />
    <div class="px-8 w-full">
       <div class="py-8 flex justify-between w-full">
      <div class="space-y-2">
        <p class="text-3xl font-semibold">Welcome, Jonathan</p>
        <p class="text-[#475467]">
          View assessments and top scorers at a glance.
        </p>
      </div>
      <div class="relative space-y-2">
        <div class="flex bg-[#00AEF8] w-fit h-fit rounded-lg items-center py-2 px-4 space-x-2 cursor-pointer" @click="toggleDropDown">
        <p class="text-sm font-medium text-white">Create assessment</p>
        <ChevronDownIcon class="text-white text-2xl" />
      </div>
      <div class="bg-white rounded-lg font-medium p-1 text-sm h-fit shadow-lg" :class="[dropDown? 'absolute' : 'hidden']" >
        <p class="p-3 hover:bg-[#F9FAFB] rounded-lg">New assessment</p>
        <p class="p-3 hover:bg-[#F9FAFB] rounded-lg whitespace-nowrap">SimplifiedUX workbook</p>
      </div>
      </div>
    </div>
    <RouterView />
    </div>
  </div>
</template>
