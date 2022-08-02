<template>
  <v-container>
    <v-card>
      <v-tabs v-model="tab" background-color="primary">
        <v-tab value="one">crypto</v-tab>
        <v-tab value="two">forex</v-tab>
        <v-tab value="three">stocks</v-tab>
      </v-tabs>

      <v-card-text>
        <v-window v-model="tab">
          <v-window-item value="one">
            crypto
          </v-window-item>

          <v-window-item value="two">
            forex
          </v-window-item>

          <v-window-item value="three">
            stocks
          </v-window-item>
        </v-window>
      </v-card-text>
    </v-card>
  </v-container>
</template>

<script>

export default {
  name: 'HelloWorld',

  data: () => ({
    tab: null,
  }),
}
</script>
