<template>
    <div class="flex w-full h-full min-h-screen bg-[#f2f4f7]">
        <Sidebar />
        <div class="w-full">
            <NavBarComponent />
            <div class="w-full pt-9 px-7">
                <div class="w-full flex items-center justify-between">
                    <p class="text-3xl font-semibold">Redirects</p>
                    <div class="flex gap-4">
                        <button class="rounded-lg shadow-md bg-white w-12 h-12 flex items-center justify-center">
                            <ServerIconComponent />
                        </button>

                        <button class="rounded-lg shadow-md bg-white w-12 h-12 flex items-center justify-center">
                            <PieChartIconComponent />
                        </button>

                        <button class="rounded-lg shadow-md bg-white w-12 h-12 flex items-center justify-center">
                            <TrendingUpIconComponent />
                        </button>

                        <button class="bg-[#1C6DB6] px-5 py-3 rounded-lg text-white font-semibold shadow-md">
                            New Redirect
                        </button>
                    </div>
                </div>
                <div class="pt-9">
                    <ListControlComponent />
                </div>
                <div class="pt-6 gap-4 flex flex-col">
                    <CardComponent />
                    <CardComponent />
                </div>
            </div>
        </div>
    </div>
</template>

<script lang="ts">
import { defineComponent } from "vue";
import Sidebar from "@/components/sidebar/SidebarComponent.vue";
import NavBarComponent from '@/components/nav-bar/NavBarComponent.vue';
import CardComponent from '@/components/redirects/CardComponent.vue';
import ServerIconComponent from '@/components/icons/ServerIconComponent.vue';
import PieChartIconComponent from '@/components/icons/PieChartIconComponent.vue';
import TrendingUpIconComponent from '@/components/icons/TrendingUpIconComponent.vue';
import ListControlComponent from "@/components/redirects/ListControlComponent.vue";

export default defineComponent({
    components: {
        Sidebar,
        NavBarComponent,
        CardComponent,
        ServerIconComponent,
        PieChartIconComponent,
        TrendingUpIconComponent,
        ListControlComponent,
    },
    setup() {
        return {};
    }
});
</script>