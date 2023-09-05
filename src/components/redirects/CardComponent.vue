<template>
  <div class="w-full bg-white rounded-lg p-6 flex gap-4">
    <div class="flex gap-3">
      <input type="checkbox" class="w-5 h-5 border border-[#D0D5DD] mt-2" />
      <div class="w-10 h-10 overflow-hidden rounded-full border border-[#EAECF0]">
        <img src="/logo.png" class="w-full h-full object-cover" />
      </div>
    </div>
    <div class="w-full">
      <div class="flex justify-between items-center">
        <p class="truncate text-[#667085] text-lg">
          Redirhub Name Line
        </p>
        <div class="flex justify-between items-center">
          <div class="flex gap-6 mr-10">
            <div class="flex items-center justify-center gap-2">
              <ActivityIconComponent class="w-5 h-5" />
              <p class="text-sm">2 clicks</p>
            </div>
            <div class="flex items-center justify-center gap-2">
              <CommandIconComponent class="w-5 h-5" />
              <p class="text-sm text-[#667085]">Permanent 301</p>
            </div>
            <div class="flex items-center justify-center gap-2">
              <CalendarIconComponent class="w-5 h-5" />
              <p class="text-sm text-[#667085]">16.08.2023</p>
            </div>
          </div>
          <div class="flex gap-4">
            <button class="w-10 h-10 bg-white rounded-lg border border-[#D0D5DD] flex items-center justify-center">
              <CopyIconComponent />
            </button>
            <button class="w-10 h-10 bg-white rounded-lg border border-[#D0D5DD] flex items-center justify-center">
              <EditIconComponent />
            </button>
            <button class="w-10 h-10 bg-white rounded-lg border border-[#D0D5DD] flex items-center justify-center">
              <MoreIconComponent />
            </button>
          </div>
        </div>
      </div>
      <div class="w-full flex items-center justify-between gap-4 my-6">
        <input class="w-full border border-[#D0D5DD] px-3 py-1 rounded-lg" />
        <ArrowRightCircleIconComponent class="w-14" />
        <input class="w-full border border-[#D0D5DD] px-3 py-1 rounded-lg" />
      </div>
    </div>
  </div>
</template>

<script lang="ts">
import { defineComponent } from 'vue';
import ActivityIconComponent from '@/components/icons/ActivityIconComponent.vue'
import ArrowRightCircleIconComponent from '@/components/icons/ArrowRightCircleIconComponent.vue'
import CommandIconComponent from '@/components/icons/CommandIconComponent.vue'
import CalendarIconComponent from '@/components/icons/CalendarIconComponent.vue'
import CopyIconComponent from '@/components/icons/CopyIconComponent.vue'
import EditIconComponent from '@/components/icons/EditIconComponent.vue'
import MoreIconComponent from '@/components/icons/MoreIconComponent.vue'


export default defineComponent({
  components: {
    ActivityIconComponent,
    ArrowRightCircleIconComponent,
    CommandIconComponent,
    CalendarIconComponent,
    CopyIconComponent,
    EditIconComponent,
    MoreIconComponent,
  },
  setup() {
    return {};
  }
})
</script>