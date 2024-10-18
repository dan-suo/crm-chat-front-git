<template>
  <v-app>
    <AppNavigation />
    <v-main>
      <router-view />
    </v-main>
  </v-app>
</template>

<script setup>
  import AppNavigation from '@/components/app/AppNavigation.vue';
</script>
