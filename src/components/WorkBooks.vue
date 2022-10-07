<script setup>
import BoxSearchIcon from "./icons/BoxSearchIcon.vue";
import EllipsisIcon from "./icons/EllipsisIcon.vue";
import PlusIcon from "./icons/PlusIcon.vue";
import TypographyIcon from "./icons/TypographyIcon.vue";
import MonitorIcon from "./icons/MonitorIcon.vue";
import ShareIcon from "./icons/ShareIcon.vue";
import PenIcon from "./icons/PenIcon.vue";
import DeleteIcon from "./icons/DeleteIcon.vue";
import { ref } from "vue";

const uxMenu = ref(false);
function toggleUxMenu() {
    uxMenu.value = !uxMenu.value;
}

const uiMenu = ref(false);
function toggleUiMenu() {
    uiMenu.value = !uiMenu.value;
}

const typographyMenu = ref(false);
function toggleTypography() {
    typographyMenu.value = !typographyMenu.value
}

</script>

<template>
  <div class="w-full space-y-6">
    <p class="text-xl font-medium text-[#344054]">Recent workbooks</p>
    <div class="flex space-x-8">
      <div class="bg-white rounded-lg p-4 shadow space-y-4 relative w-fit">
        <div class="flex justify-between items-start">
          <div class="flex space-x-4 items-end">
            <div class="bg-[#F040371A] rounded-[10px] p-6">
              <BoxSearchIcon class="text-5xl text-[#F04037]" />
            </div>
            <div class="space-y-1">
              <p class="font-semibold text-[#344054]">UX Research</p>
              <p class="text-sm text-[#344054]">25 questions</p>
              <p class="text-sm text-[#344054]">30 minutes</p>
            </div>
          </div>
          <EllipsisIcon class="text-[#00AEF8] text-2xl cursor-pointer" @click="toggleUxMenu" />
        </div>
        <p class="text-sm text-[#344054]">
          Contains questions that will help improve your design thinking process
          to enhance your UX design.
        </p>
        <div class="pt-2 border-t-2 border-t-[#D0D5DD] w-full">
          <div class="relative w-full">
            <img src="../assets/images/image1.png" class="w-10" />
            <img
              src="../assets/images/image2.png"
              class="w-10 absolute left-6 top-0"
            />
            <img
              src="../assets/images/image3.png"
              class="w-10 absolute left-12 top-0"
            />
            <img
              src="../assets/images/image4.png"
              class="w-10 absolute left-[25%] top-0"
            />
            <img
              src="../assets/images/image5.png"
              class="w-10 absolute left-[34%] top-0"
            />
            <p
              class="
                bg-[#F2F4F7]
                text-[#475467]
                pt-1
                pb-2
                px-3
                rounded-3xl
                absolute
                top-1
                left-[43%]
                text-sm
                font-medium
              "
            >
              +120 results
            </p>
          </div>
        </div>
        <div class="bg-white border p-1 border-[#F9FAFB] space-y-1 shadow-lg rounded-lg w-[65%] right-3 top-6" :class="[uxMenu ? 'absolute' : 'hidden']">
            <div class="flex space-x-2 rounded-lg items-center hover:bg-[#F9FAFB] p-2">
                <ShareIcon class="text-base" />
                <p class="font-medium text-sm">Share workbook</p>
            </div>
            <div class="flex space-x-2 rounded-lg items-center hover:bg-[#F9FAFB] p-2">
                <PenIcon class="text-base" />
                <p class="font-medium text-sm">Edit workbook</p>
            </div>
            <div class="flex space-x-2 rounded-lg items-center hover:bg-[#F9FAFB] p-2">
                <DeleteIcon class="text-base" />
                <p class="font-medium text-sm">Delete workbook</p>
            </div>
        </div>
      </div>

      <div class="bg-white rounded-lg p-4 shadow space-y-4 relative">
        <div class="flex items-start justify-between">
          <div class="flex space-x-4 items-end">
            <div class="bg-[#E3F0FF] rounded-[10px] p-6">
              <MonitorIcon class="text-5xl" />
            </div>
            <div class="space-y-1">
              <p class="font-semibold text-[#344054]">UX Principle</p>
              <p class="text-sm text-[#344054]">25 questions</p>
              <p class="text-sm text-[#344054]">30 minutes</p>
            </div>
          </div>
          <EllipsisIcon class="text-[#00AEF8] text-2xl cursor-pointer" @click="toggleUiMenu" />
        </div>
        <p class="text-sm text-[#344054]">
          Contains questions that will help improve your design thinking process
          to enhance your UX design.
        </p>
        <div class="pt-2 border-t-2 border-t-[#D0D5DD] w-full">
          <div class="relative w-full">
            <img src="../assets/images/image1.png" class="w-10" />
            <img
              src="../assets/images/image2.png"
              class="w-10 absolute left-6 top-0"
            />
            <img
              src="../assets/images/image3.png"
              class="w-10 absolute left-12 top-0"
            />
            <img
              src="../assets/images/image4.png"
              class="w-10 absolute left-[25%] top-0"
            />
            <img
              src="../assets/images/image5.png"
              class="w-10 absolute left-[34%] top-0"
            />
            <p
              class="
                bg-[#F2F4F7]
                text-[#475467]
                pt-1
                pb-2
                px-3
                rounded-3xl
                absolute
                top-1
                left-[43%]
                text-sm
                font-medium
              "
            >
              +83 results
            </p>
          </div>
        </div>
        <div class="bg-white border p-1 border-[#F9FAFB] space-y-1 shadow-lg rounded-lg w-[65%] right-3 top-6" :class="[uiMenu ? 'absolute' : 'hidden']">
            <div class="flex space-x-2 rounded-lg items-center hover:bg-[#F9FAFB] p-2">
                <ShareIcon class="text-base" />
                <p class="font-medium text-sm">Share workbook</p>
            </div>
            <div class="flex space-x-2 rounded-lg items-center hover:bg-[#F9FAFB] p-2">
                <PenIcon class="text-base" />
                <p class="font-medium text-sm">Edit workbook</p>
            </div>
            <div class="flex space-x-2 rounded-lg items-center hover:bg-[#F9FAFB] p-2">
                <DeleteIcon class="text-base" />
                <p class="font-medium text-sm">Delete workbook</p>
            </div>
        </div>
      </div>

      <div class="bg-white rounded-lg p-4 shadow relative space-y-4">
        <div class="flex items-start justify-between">
          <div class="flex space-x-4 items-end">
            <div class="bg-[#FDECFF] rounded-[10px] p-6">
              <TypographyIcon class="text-5xl" />
            </div>
            <div class="space-y-1">
              <p class="font-semibold text-[#344054]">Typography</p>
              <p class="text-sm text-[#344054]">25 questions</p>
              <p class="text-sm text-[#344054]">30 minutes</p>
            </div>
          </div>
          <EllipsisIcon class="text-[#00AEF8] text-2xl cursor-pointer" @click="toggleTypography" />
        </div>
        <p class="text-sm text-[#344054]">
          Used space Contains questions that will help improve your typographic
          skill to enhance your designs.
        </p>
        <div class="pt-2 border-t-2 border-t-[#D0D5DD] w-full">
          <div class="relative w-full">
            <img src="../assets/images/image1.png" class="w-10" />
            <img
              src="../assets/images/image2.png"
              class="w-10 absolute left-6 top-0"
            />
            <img
              src="../assets/images/image3.png"
              class="w-10 absolute left-12 top-0"
            />
            <img
              src="../assets/images/image4.png"
              class="w-10 absolute left-[25%] top-0"
            />
            <img
              src="../assets/images/image5.png"
              class="w-10 absolute left-[34%] top-0"
            />
            <p
              class="
                bg-[#F2F4F7]
                text-[#475467]
                pt-1
                pb-2
                px-3
                rounded-3xl
                absolute
                top-1
                left-[43%]
                text-sm
                font-medium
              "
            >
              +12 results
            </p>
          </div>
        </div>
        <div class="bg-white border p-1 border-[#F9FAFB] space-y-1 shadow-lg rounded-lg w-[65%] right-3 top-6" :class="[typographyMenu ? 'absolute' : 'hidden']">
            <div class="flex space-x-2 rounded-lg items-center hover:bg-[#F9FAFB] p-2">
                <ShareIcon class="text-base" />
                <p class="font-medium text-sm">Share workbook</p>
            </div>
            <div class="flex space-x-2 rounded-lg items-center hover:bg-[#F9FAFB] p-2">
                <PenIcon class="text-base" />
                <p class="font-medium text-sm">Edit workbook</p>
            </div>
            <div class="flex space-x-2 rounded-lg items-center hover:bg-[#F9FAFB] p-2">
                <DeleteIcon class="text-base" />
                <p class="font-medium text-sm">Delete workbook</p>
            </div>
        </div>
      </div>
      <div class="bg-white flex rounded-lg p-4 shadow space-y-4">
        <div class="flex space-x-3 items-center">
          <PlusIcon class="text-2xl text-[#00AEF8]" />
          <p class="text-[#00AEF8] font-medium text-sm whitespace-nowrap w-fit">
            2 more
          </p>
        </div>
      </div>
    </div>
  </div>
</template>
