<template>
  <v-app>
    <Menu />
    <v-main>
      <router-view />
    </v-main>

    <AppFooter />
  </v-app>
</template>

<script setup>
  import Menu from '@/layouts/Menu.vue';
</script>
