<template>
  <div class="fill-height grid">
    <div >
      <ChatContactList />
    </div>
    <div>Messages</div>
    <div>Info</div>
  </div>
</template>

<script setup>
import ChatContactList from "@/components/chat/contacts/ChatContactList.vue";
</script>

<style scoped>
.grid {
  display: grid;
  grid-template-columns: 1fr 2fr 1fr;
  width:100%;
}
</style>
