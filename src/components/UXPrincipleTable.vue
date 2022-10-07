<script setup>
import ChevronRightIcon from './icons/ChevronRightIcon.vue';
import ChevronUpIcon from './icons/ChevronUpIcon.vue';
import { ref } from 'vue';

const collapse = ref(false)
function toggleCollapse() {
    collapse.value = !collapse.value
}
</script>
    
    <template>
        <div class="flex items-center justify-between px-6 py-2 text-[#101828] bg-[#F2F4F7]" :class="[collapse ? 'border-none' : 'border-b-2 border-b-[#EAECF0]']">
            <p class="font-semibold text-lg">UX Principle</p>
            <ChevronUpIcon class="cursor-pointer" @click="toggleCollapse" />
        </div>
        <table class="w-full" :class="[collapse ? '' : 'hidden']">
            <colgroup>
                <col span="1" style="width: 2%;">
                <col span="1" style="width: 15%;">
                <col span="1" style="width: 27%;">
                <col span="1" style="width: 24%;">
                <col span="1" style="width: 14%;">
                <col span="1" style="width: 14%;">
                <col span="1" style="width: 4%;">
            </colgroup>
            <thead  class="bg-[#F9FAFB] h-11 text-left text-xs font-thin text-[#475467]">
                <tr>
                    <th></th>
                    <th>Name</th>
                    <th>Email Address</th>
                    <th>Role</th>
                    <th>Score</th>
                    <th>Time used</th>
                    <th></th>
                </tr>
            </thead>
            <tbody>
                <tr class="border-t h-[70px] text-left border-t-[#EAECF0] text-[#475467] text-sm">
                    <td></td>
                    <td class="font-medium text-[#101828]">Olivia Rhye</td>
                    <td>olivia@untitledui.com</td>
                    <td>Product Design</td>
                    <td>95%</td>
                    <td>7:29</td>
                    <td><ChevronRightIcon /></td>
                </tr>
                <tr class="border-t h-[70px] text-left border-t-[#EAECF0] text-[#475467] text-sm">
                    <td></td>
                    <td class="font-medium text-[#101828]">Demi Wilkinson</td>
                    <td>demi@untitledui.com</td>
                    <td>Backend Developer</td>
                    <td>95%</td>
                    <td>19:30</td>
                    <td><ChevronRightIcon /></td>
                </tr>
                <tr class="border-t h-[70px] text-left border-t-[#EAECF0] text-[#475467] text-sm">
                    <td></td>
                    <td class="font-medium text-[#101828]">Candice Wu</td>
                    <td>candice@untitledui.com</td>
                    <td>Fullstack Developer</td>
                    <td>90%</td>
                    <td>21:45</td>
                    <td><ChevronRightIcon /></td>
                </tr>
            </tbody> 
        </table>
    </template>