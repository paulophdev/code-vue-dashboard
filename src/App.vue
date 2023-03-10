<template>
  <div class="flex">
    <!-- Sidebar -->
    <div
      class="absolute left-0 w-3/12 h-screen bg-gray-700 z-[1035] lg:sticky lg:top-0"
      :style="myStyle"
      id="sidenav-1"
      data-te-sidenav-init
      data-te-sidenav-hidden="false"
      :data-te-sidenav-mode="sidenavMod"
      data-te-sidenav-content="#content"
    >
      <VueSidebar />
    </div>
    <!-- /. Sidebar -->

    <div class="w-full" id="content">
      <!-- Menu Header -->
      <VueHead />

      <!-- Content -->
      <div class="p-10 overflow-auto bg-white h-screen">
        <VueDashboard />
      </div>
    </div>
  </div>
</template>

<script>
import VueHead from "@/components/VueHead.vue";
import VueSidebar from "@/components/VueSidebar.vue";
import VueDashboard from "@/pages/VueDashboard.vue";

export default {
  name: "App",
  components: {
    VueSidebar,
    VueHead,
    VueDashboard,
  },
  computed: {
    myStyle() {
      return window.innerWidth <= 768
        ? {
            transform: "translateX(-100%)",
            top: "76px",
          }
        : "";
    },
    sidenavMod() {
      return window.innerWidth <= 768 ? "over" : "side";
    },
  },
};
</script>

<style>
body {
  background-color: #dcdcdc;
}
</style>
