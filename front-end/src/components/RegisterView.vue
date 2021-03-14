<template>
  <v-card>
    <v-card-title>
      Register
    </v-card-title>
    <v-card-text>
      <RegisterInput label="Username"/>
      <RegisterInput :password="true" label="Password"/>
      <RegisterInput :password="true" label="Confirm Password"/>
    </v-card-text>
    <v-card-actions>
      <v-btn>
        Submit
      </v-btn>
    </v-card-actions>
  </v-card>
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

