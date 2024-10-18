<template>
  <v-card
    class="pa-2"
    height="100%"
  >
  <v-text-field
    label="Начать поиск"
    placeholder="Ищем ..."
    variant="outlined"
    class="mt-4 mx-4"
  >
  </v-text-field>

  <div class="overflow-auto" >
    <v-list>
      <v-list-subheader>Мои диалоги</v-list-subheader>

      <v-list-item
        v-for="(item, i) in items"
        :key="i"
        :value="item"
        color="primary"
        rounded="xl"
      >
        <template v-slot:prepend>
          <v-icon :icon="item.icon"></v-icon>
        </template>

        <v-list-item-title>{{ item.text }}</v-list-item-title>
      </v-list-item>
    </v-list>
  </div>
  </v-card>
</template>

<script>
  export default {
    data: () => ({
      items: [
        { text: 'Real-Time', icon: 'mdi-clock' },
        { text: 'Audience', icon: 'mdi-account' },
        { text: 'Conversions', icon: 'mdi-flag' },
      ],
    }),
  }
</script>