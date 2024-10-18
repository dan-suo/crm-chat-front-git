<template>
  <div class="fill-height grid">
    <div>
      <ChatContactList />
    </div>
    <div>
      <ChatMessages />
    </div>
    <div>
      <chat-contact-info />
    </div>
  </div>
</template>

<script setup>
import ChatContactList from "@/components/chat/contacts/ChatContactList.vue";
</script>

<style scoped>
.grid {
  display: grid;
  grid-template-columns: 1fr 2fr 1fr;
  width: 100%;
}

.left-0 {
  left:0;
}
</style>
