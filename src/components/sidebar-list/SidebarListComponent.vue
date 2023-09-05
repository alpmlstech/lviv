<template>
  <ul class="w-full pt-3">
    <li class="" v-for="item in list" :key="item.title">
      <a class="flex gap-6 py-3 px-6 hover:bg-[#F2F4F7] transition-all duration-200" :href="item.url">
        <component :is="item.icon">
        </component>
        <p class="text-base">{{ item.title }}</p>
      </a>
    </li>
  </ul>
</template>

<script lang="ts">
import { defineComponent, markRaw } from 'vue';
import HomeIconComponent from '../icons/HomeIconComponent.vue';
import ShuffleIconComponent from '../icons/ShuffleIconComponent.vue';
import LinkIconComponent from '../icons/LinkIconComponent.vue';
import EyeIconComponent from '../icons/EyeIconComponent.vue';

import ServerIconComponent from '../icons/ServerIconComponent.vue';
import CoinStackIconComponent from '../icons/CoinStackIconComponent.vue';
import SettingsIconComponent from '../icons/SettingsIconComponent.vue';

const list = [
  {
    icon: markRaw(HomeIconComponent),
    title: 'Home',
    url: '#home',
  },
  {
    icon: markRaw(ShuffleIconComponent),
    title: 'Redirects',
    url: '#home',
  },
  {
    icon: markRaw(LinkIconComponent),
    title: 'URL shortener',
    url: '#home',
  },
  {
    icon: markRaw(EyeIconComponent),
    title: 'Monitor',
    url: '#home',
  },
  {
    icon: markRaw(ServerIconComponent),
    title: 'Hostnames',
    url: '#home',
  },
  {
    icon: markRaw(CoinStackIconComponent),
    title: 'Subscriptions',
    url: '#home',
  },
  {
    icon: markRaw(SettingsIconComponent),
    title: 'Settings',
    url: '#home',
  },
]

export default defineComponent({
  components: {
    // eslint-disable-next-line vue/no-unused-components
    HomeIconComponent,
  },
  data() {
    return {
      list,
    }
  },
  setup: () => {
    return {};
  }
})


</script>