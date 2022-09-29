<template>
  <v-app style="{ background: $vuetify.theme.thems.light.background }">
    <v-layout row>
      <v-flex md8>
        <v-app
          style="{ background: $vuetify.theme.thems.dark.background }"
          class="rounded-tr-xl rounded-br-xl"
        >
        <v-container>
          
        </v-container>
        </v-app>
      </v-flex>
      <v-flex md4>
        <v-app style="{ background: $vuetify.theme.thems.light.background }">
          <v-container>

          </v-container>
        </v-app>
      </v-flex>
    </v-layout>
  </v-app>
</template>

<script>
export default {
  data: () => ({
    width: 2,
    radius: 10,
    padding: 8,
    linecap: "round",
    value: [0, 2, 5, 9, 5, 10, 3, 5, 0, 0, 1, 8, 2, 9, 0],
    fill: false,
    type: "trend",
    autoLineWidth: false,
  }),
  computed: {
    theme() {
      return this.$vuetify.them.dark ? "dark" : "light";
    },
  },
};
</script>
