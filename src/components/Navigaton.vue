<template>
    <v-navigation-drawer
      app
    >
        <v-list-item-group>
            <v-list-item
              v-for="item in nav"
              :key="item.id"
            >
              {{item.text}}
            </v-list-item>
        </v-list-item-group>
    </v-navigation-drawer>
</template>

<script>
export default {
  name: 'Navigation',
  data: () => ({
    nav: [
      { text: 'Оголошення', id: 'main' },
      { text: 'Новини', id: 'news' },
      { text: 'Правила', id: 'rules' }
    ]
  })
}
</script>
