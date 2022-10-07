<script setup>
import ChevronUpIcon from "./icons/ChevronUpIcon.vue";
import UXResearchTable from "./UXResearchTable.vue";
import UXPrincipleTable from "./UXPrincipleTable.vue";
import TypographyTable from "./TypographyTable.vue";
</script>

<template>
    <div class="w-full space-y-6">
    <p class="text-xl font-semibold text-[#344054]">Recent results</p>
    <div class="bg-white rounded-lg pt-4 shadow-md">
        <div class="space-y-2 px-6 mb-6">
            <p class="text-lg font-semibold text-[#101828]">Top 3 scorers</p>
            <p class="text-sm text-[#344054]">See the top scorers within each workbook</p>
        </div>
        <UXResearchTable />
        <UXPrincipleTable />
        <TypographyTable />
    </div>
    </div>
</template>