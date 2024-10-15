<template>
  <v-app>
    <v-main>
      <Menu />
      <router-view />
    </v-main>

    <AppFooter />
  </v-app>
</template>

<script setup>
  import Menu from '@/layouts/Menu.vue';
</script>
