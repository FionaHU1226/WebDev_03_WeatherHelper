<template>
  <div class="flex flex-col min-h-screen font-Roboto bg-waether-primary">
    <SiteNavigation />
    <RouterView />
  </div>
</template>

<script setup>
import { Routview } from "vue-router";
import SiteNavigation from "./components/SiteNavigation.vue";
</script>

<style lang="scss" scoped>
</style>