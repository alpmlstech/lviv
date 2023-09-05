<template>
  <div class="w-full flex px-7 items-center justify-between h-16 border-b border-b-[#EAECF0] bg-white">
    <div class="flex gap-4">
      <SearchIconComponent />
      <input placeholder="Search" />
    </div>
    <div class="flex items-center gap-4 cursor-pointer">
      <img src="/Avatar.png" class="w-10 h-10 object-cover rounded-full" />
      <p>John Smith</p>
      <ChevronDownIcon />
    </div>
  </div>
</template>

<script lang="ts">
import { defineComponent } from 'vue';
import SearchIconComponent from '../icons/SearchIconComponent.vue';
import ChevronDownIcon from '../icons/ChevronDownIcon.vue';

export default defineComponent({
  components: {
    SearchIconComponent,
    ChevronDownIcon
  },
  setup() {
    return {

    };
  }
});

</script>