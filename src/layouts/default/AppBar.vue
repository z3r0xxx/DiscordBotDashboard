<template>
  <v-toolbar absolute="true" flat="true" density="default">
    <v-toolbar-title>
      <v-btn rounded="xl">
        RinoBot
      </v-btn>
    </v-toolbar-title>

    <v-btn class="ml-2" rounded="xl" prepend-icon="mdi-book-open-variant">
      Документация
    </v-btn>
    <v-btn class="ml-2" rounded="xl" prepend-icon="mdi-console-line">
      Команды
    </v-btn>
    <v-btn class="ml-2" rounded="xl" prepend-icon="mdi-chart-areaspline">
      Статистика
    </v-btn>
    <v-btn class="ml-2" rounded="xl" prepend-icon="mdi-store">
      Наш мерч
    </v-btn>

    <v-spacer />

    <v-menu min-width="200px" rounded>
      <template v-slot:activator="{ props }">
        <v-btn class="ml-2 mr-3" icon v-bind="props">
          <v-avatar><v-img src="https://cdn.discordapp.com/avatars/637297397600616461/1bed5fd68a37f7ac044fea8ac77577dd.png" alt="zrx"></v-img></v-avatar>
        </v-btn>
      </template>

      <v-card
        class="mx-auto"
        width="300"
        rounded="xl"
        title="zrx"
        subtitle="z3r0x1ch"
      >
        <template v-slot:prepend>
          <v-avatar><v-img src="https://cdn.discordapp.com/avatars/637297397600616461/1bed5fd68a37f7ac044fea8ac77577dd.png" alt="zrx"></v-img></v-avatar>
        </template>
        <v-divider></v-divider>

        <v-list>
          <v-list-item value="item">
            <template v-slot:prepend>
              <v-icon icon="mdi-server"></v-icon>
            </template>

            <v-list-item-title>Мои серверы</v-list-item-title>
          </v-list-item>
          <v-list-item value="item">
            <template v-slot:prepend>
              <v-icon icon="mdi-card-account-details"></v-icon>
            </template>

            <v-list-item-title>Карточка рейтинга</v-list-item-title>
          </v-list-item>
          <v-list-item value="item">
            <template v-slot:prepend>
              <v-icon icon="mdi-logout"></v-icon>
            </template>

            <v-list-item-title>Выйти</v-list-item-title>
          </v-list-item>
        </v-list>
        
        <v-divider></v-divider>

        <v-list>
          <v-list-item value="item">
            <template v-slot:prepend>
              <v-icon icon="mdi-chat-question"></v-icon>
            </template>

            <v-list-item-title>Получить помощь</v-list-item-title>
          </v-list-item>
        </v-list>
      </v-card>

    </v-menu>
    
  </v-toolbar>
</template>

  
      

<script>
  export default {
    data: () => ({
      user: {
        initials: 'JD',
        fullName: 'John Doe',
        email: 'john.doe@doe.com',
      },
    }),
  }
</script>