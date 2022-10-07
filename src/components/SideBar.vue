<script setup>
import DashboardIcon from './icons/DashboardIcon.vue';
import UserIcon from './icons/UserIcon.vue';
import SupportIcon from './icons/SupportIcon.vue';
import SettingsIcon from './icons/SettingsIcon.vue';
import AvatarIcon from './icons/AvatarIcon.vue';
import LogoutIcon from './icons/LogoutIcon.vue';
</script>

<template>
  <aside
    class="sticky overflow-hidden top-0 left-0 bg-white border-r border-r-gray-200 h-full w-[21vw]"
  >
    <div class="px-6 space-y-16">
      <p class="text-white 2xl">Logo</p>
      <div class="space-y-4">
        <div class="flex space-x-2 items-center">
        <DashboardIcon class="text-2xl text-[#119CD8]" />
        <router-link class="text-[#119CD8] font-semibold text-[16px]" to="/">Dashboard</router-link>
      </div>
      <div class="flex space-x-2 items-center">
        <UserIcon class="text-2xl text-[#667085]" />
        <p class="text-[16px] font-semibold">Teams</p>
      </div>
      </div>
    </div>
    <footer class="absolute bottom-0 left-0 px-3 space-y-6">
        <div class="px-3 space-y-4">
        <div class="flex space-x-2 items-center">
        <SupportIcon class="text-2xl text-[#667085]" />
        <p class="font-semibold text-[16px]">Support</p>
      </div>
      <div class="flex space-x-2 items-center">
        <SettingsIcon class="text-2xl text-[#667085]" />
        <p class="text-[16px] font-semibold">Settings</p>
      </div>
      </div>
      <div class="bg-[#F2F4F7] rounded-lg space-y-1 px-3 py-4">
        <p class="font-semibold text-sm">Need more than one workbook?</p>
        <p class="text-sm">
            Upgrade your plan for a slow as $59.99/m create unlimited workbooks
        </p>
        <div class="flex space-x-2 pt-4">
            <p class="font-semibold text-sm">Remind me later</p>
            <p class="font-semibold text-sm text-[#00AEF8]">Upgrade now</p>
        </div>
      </div>
      <div class="border-t-2 border-t-[#F2F4F7] px-1 pt-4 pb-6 flex items-center space-x-2 relative">
        <img src="../assets/images/Avatar.png" />
        <div class="text-sm">
            <p class="font-semibold">Jonathan Smith</p>
            <p>js27@jusacut.com</p>
        </div>
        <LogoutIcon class="text-2xl absolute top-4 right-1 text-[#667085]" />
      </div>
    </footer>
  </aside>
</template>
