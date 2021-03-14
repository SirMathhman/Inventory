<template>
  <v-app>
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
