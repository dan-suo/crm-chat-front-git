<template>
    <v-navigation-drawer
        v-model="drawer"
        :rail="rail"
        permanent
        @click="rail = false"
        class="transition cursor-pointer"
      >
        <v-list-item
          prepend-avatar="https://randomuser.me/api/portraits/men/46.jpg"
          class="ml-2"
          title="Пользователь"
          nav
        >
          <template v-slot:append>
            <v-btn
              icon="mdi-chevron-left"
              variant="text"
              @click.stop="rail = !rail"
            ></v-btn>
          </template>
        </v-list-item>

        <v-divider></v-divider>

        <v-list density="compact" nav>
          <v-list-item 
            v-for="navigationItem in navigationItems" 
            :key="navigationItem.id" 
            :prepend-icon="navigationItem.icon" 
            :title="navigationItem.title" 
            :value="navigationItem.value"
            >
          </v-list-item>
        </v-list>
    </v-navigation-drawer>
</template>

<script>
  export default {
    data () {
      return {
        drawer: true,
        rail: true,
      }
    },
  }
</script>

<script setup>

  import {ref} from 'vue'

  const navigationItems = ref([
    {
      id: 1,
      title: 'Чаты',
      icon: 'mdi-text',
      value: 'chats'
    }
  ]) 
  
</script>