<template>
    <v-container fluid>
        <v-row dense>
            <v-col
                v-for="item in announsments"
                :key="item.id"
                :cols="12"
            >
                <v-card>
                        <v-card-title>{{ item.title }}</v-card-title>
                        <v-card-subtitle>{{ item.category }}</v-card-subtitle>
                        <v-card-text>{{ item.text }}</v-card-text>
                        <v-card-actions>
                            <a
                                :href="'https://t.me/' + item.from.replace('@','')"
                                target="_blank"
                                style="text-decoration: none;"
                            >
                                <v-btn outlined color="info">Звертатися до: {{ item.from }}</v-btn>
                            </a>
                        </v-card-actions>
                </v-card>
            </v-col>
        </v-row>
    </v-container>
</template>

<script>
export default {
  name: 'announsment',
  data: () => ({
    announsments: [
      {
        id: 1,
        title: 'Шукаю редактора',
        text: 'Шукаю редактора на аніме Hajime no Ippo (наразі це 50 серій, переклад триває)',
        category: 'SUB',
        from: '@MadFrenzyRabbit'
      },
      {
        id: 2,
        title: 'Потрібні сабери',
        text: 'Потрібні сабери на проект "Сомалі та Лісовий Дух".',
        category: 'SUB',
        from: '@sobad_mp4'
      },
      {
        id: 3,
        title: 'Потрібен перекладач',
        text: 'Потрібен перекладач для аніме Удаване кохання ТВ-2(Nisekoi tv-2)',
        category: 'Translate',
        from: '@Baka_shinji'
      }
    ]
  })
}
</script>
