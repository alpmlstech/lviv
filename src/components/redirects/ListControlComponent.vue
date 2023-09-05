<template>
  <div class="flex justify-between">
    <button class="flex items-center gap-2 px-4 py-2 rounded-lg shadow-md bg-white">
      Filter
      <FilterIconComponent />
    </button>

    <div class="flex items-center gap-4">
      <p>Appearance</p>
      <div class="flex">
        <button class="w-11 h-10 flex items-center justify-center border border-[#D0D5DD] rounded-l-lg">
          <AlignIconComponent />
        </button>
        <button class="w-11 h-10 flex items-center justify-center border border-[#D0D5DD] rounded-r-lg bg-white">
          <SidebarIconComponent />
        </button>
      </div>
    </div>
  </div>
</template>

<script lang="ts">
import { defineComponent } from 'vue';
import FilterIconComponent from '../icons/FilterIconComponent.vue';
import AlignIconComponent from '../icons/AlignIconComponent.vue';
import SidebarIconComponent from '../icons/SidebarIconComponent.vue';

export default defineComponent({
  components: {
    FilterIconComponent,
    AlignIconComponent,
    SidebarIconComponent
  },
  setup() {
    return {

    };
  }
})
</script>