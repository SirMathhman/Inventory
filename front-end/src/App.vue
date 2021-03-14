<template>
  <v-app>
    <v-app-bar app>
      <v-container fluid>
        <v-row align="center" justify="space-between">
          <span class="ma-0 pa-0 text-center text-h4">
            Inventory
          </span>
          <v-btn v-on:click="$vuetify.theme.dark = !$vuetify.theme.dark">
            Toggle Dark
          </v-btn>
        </v-row>
      </v-container>
    </v-app-bar>
    <v-main>
      <RegisterView></RegisterView>
    </v-main>
  </v-app>
</template>

<script lang="ts">
import Vue from "vue";
import RegisterView from "@/components/RegisterView.vue";
import {Component} from "vue-property-decorator";

@Component({
  components: {RegisterView}
})
export default class App extends Vue {
}
</script>
