<template>
  <v-app>
    <v-app-bar app>
      <v-toolbar-title class="headline text-uppercase">
        <span>2019</span>
        <span class="font-weight-light">CARP SLAM</span>
      </v-toolbar-title>
      <v-spacer></v-spacer>
      <v-btn
        text
        href="https://www.denvertu.org/"
        target="_blank"
      >
        <span class="mr-2">Denver Trout Unlimted</span>
      </v-btn>
    </v-app-bar>

    <v-content>
      <ResultsDisplay/>
    </v-content>
  </v-app>
</template>

<script>
import ResultsDisplay from './components/ResultsDisplay';

export default {
  name: 'App',
  components: {
    ResultsDisplay,
  },
  data: () => ({
    //
  }),
};
</script>
