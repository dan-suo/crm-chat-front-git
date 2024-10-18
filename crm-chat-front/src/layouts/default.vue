<template>
  <v-app>
    <AppNavigation />
    <v-main>
      <ChatList />
      <router-view />
    </v-main>
    <AppFooter />
  </v-app>
</template>

<script setup>
  import AppNavigation from '@/components/app/AppNavigation.vue';
  import ChatList from '@/components/chat/ChatList.vue';
</script>
