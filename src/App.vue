<template>

  <!-- App.vue -->

  <v-app>
    <v-navigation-drawer app>
      <!-- -->
    </v-navigation-drawer>

    <v-app-bar app>
      <!-- -->
    </v-app-bar>

    <!-- Sizes your content based upon application components -->
    <v-main>

      <!-- Provides the application the proper gutter -->
      <v-container fluid>

        <vue-calendar-checkout v-bind:reserved="reserved"></vue-calendar-checkout>

      </v-container>
    </v-main>

    <v-footer app>
      <!-- -->
    </v-footer>
  </v-app>
</template>

<script>

import CalendarCheckout from "./components/CalendarCheckout";

export default {
  name: 'App',
  components: {
    'vue-calendar-checkout': CalendarCheckout
  },
  data: () => ({
      reserved : [
        '1-1',
        '1-3',
        '1-9',
        '1-47',
        '3-1',
        '3-3',
        '3-9',
        '3-12',
      ]
  })

}
</script>

<style>
</style>
