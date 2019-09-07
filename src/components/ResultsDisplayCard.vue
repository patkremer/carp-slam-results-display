<template>
  <div>
    <v-card class="mx-auto" width="400px">
      <v-img class="white--text" height="200px" :src="carp.Picture" v-if="carp.Picture">
        <v-card-title class="align-end fill-height">{{carp.Species}} - {{carp.Length}} inches</v-card-title>
      </v-img>
      <v-card-title class="align-end fill-height" v-else>{{carp.Species}} - {{carp.Length}} inches</v-card-title>
      <v-card-text></v-card-text>
      <v-card-text>
        Team: {{carp.Team}}
        <br>
        Caught By: {{carp.Competitor}} at {{carp.Time}}
        <br>
        Beat: {{carp.Beat}}
      </v-card-text>
    </v-card>
  </div>
</template>

<script>
export default {
  props: {
    carp: Object
  },
  data: () => ({})
};
</script>
