<template>
  <v-text-field :label="label"
                :type="password ? 'password' : 'text'"
                clearable
                dense
                outlined>
  </v-text-field>
</template>
<script lang="ts">
import {Component, Prop, Vue} from "vue-property-decorator";

@Component({})
export default class RegisterInput extends Vue {
  @Prop({required: true})
  private readonly label: string;

  @Prop({default: false})
  private readonly password: boolean;
}
</script>
