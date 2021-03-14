<template>
  <v-container class="fill-height">
    <v-row align="center" justify="center">
      <v-col>
        <v-card>
          <v-card-title>
            <v-container>
              <v-row align="center" justify="center">
                <span class="text-center ma-7 pa-0 text-h1">
                  Register
                </span>
              </v-row>
            </v-container>
          </v-card-title>
          <v-card-text>
            <RegisterInput label="Username"/>
            <RegisterInput :password="true" label="Password"/>
            <RegisterInput :password="true" label="Confirm Password"/>
          </v-card-text>
          <v-card-actions>
            <v-btn block>
              Submit
            </v-btn>
          </v-card-actions>
        </v-card>
      </v-col>
    </v-row>
  </v-container>
</template>

<script lang="ts">
import {Component, Vue} from "vue-property-decorator";
import RegisterInput from "@/components/RegisterInput.vue";

@Component({
  components: {RegisterInput}
})
export default class RegisterView extends Vue {

}
</script>
<style scoped>
</style>
