<template>
  <v-container>
    <v-layout text-center wrap>
      <v-flex mb-4>
        <h1 class="display-2 font-weight-bold mb-3">Carp Slam 2019 Results</h1>
      </v-flex>

      <v-flex mb-12 xs12>
        <h2 class="headline font-weight-bold mb-3">Morning Results</h2>

        <v-layout>
          <v-row no-gutters>
            <v-col v-for="(carp, i) in carpSlamResults.morning" :key="i">
              <ResultsDisplayCard v-bind:carp="carp"></ResultsDisplayCard>
            </v-col>
          </v-row>
        </v-layout>
      </v-flex>
    </v-layout>
  </v-container>
</template>

<script>
import ResultsDisplayCard from "./ResultsDisplayCard.vue";
export default {
  components: {
    ResultsDisplayCard
  },
  data: () => ({
    carpSlamResults: {
      morning: [
        {
          Team: "Clifton-Janine Whispell",
          Competitor: "Clifton",
          Beat: "Cuernavaca -H",
          Species: "Carp",
          Time: [10, 23, 0, 0].join(":"),
          Length: 18.5,
          "Total Carp Inches": null,
          "Team Carp Inches": null,
          Picture: ""
        },
        {
          Team: "Connor-Laurenti",
          Competitor: "Connor",
          Beat: "104th Hi -D",
          Species: "Carp",
          Time: [10, 45, 0, 0].join(":"),
          Length: 29.5,
          "Total Carp Inches": null,
          "Team Carp Inches": null,
          Picture: "https://i.imgur.com/8UihtmV.jpg"
        },
        {
          Team: "Kolanda-Graeve",
          Competitor: "Kolanda",
          Beat: "Sand Creek -G",
          Species: "Carp",
          Time: [9, 27, 0, 0].join(":"),
          Length: 18.25,
          "Total Carp Inches": null,
          "Team Carp Inches": null,
          Picture: "" //
        },
        {
          Team: "Kolanda-Graeve",
          Competitor: "Kolanda",
          Beat: "Sand Creek -G",
          Species: "Carp",
          Time: [11, 10, 0, 0].join(":"),
          Length: 27.25,
          "Total Carp Inches": null,
          "Team Carp Inches": null,
          Picture: ""
        },
        {
          Team: "Mikesell-Nickolas",
          Competitor: "Mikesell",
          Beat: "120th Hi -B",
          Species: "Carp",
          Time: [11, 24, 0, 0].join(":"),
          Length: 24,
          "Total Carp Inches": null,
          "Team Carp Inches": null,
          Picture: "https://i.imgur.com/Rkutxia.jpg"
        },
        {
          Team: "Mikesell-Nickolas",
          Competitor: "Mikesell",
          Beat: "120th Hi -B",
          Species: "Carp",
          Time: [10, 25, 0, 0].join(":"),
          Length: 26.5,
          "Total Carp Inches": null,
          "Team Carp Inches": null,
          Picture: "https://i.imgur.com/eCTSnA3.png"
        },
        {
          Team: "Mikesell-Nickolas",
          Competitor: "Nickolas",
          Beat: "120th Hi -B",
          Species: "Carp",
          Time: [9, 50, 0, 0].join(":"),
          Length: 29.5,
          "Total Carp Inches": null,
          "Team Carp Inches": null,
          Picture: "https://i.imgur.com/zoo1EDw.png"
        },
        {
          Team: "Smethurst-Putzier",
          Competitor: "Marshall",
          Beat: "120th Low -A",
          Species: "Carp",
          Time: [9, 40, 0, 0].join(":"),
          Length: 27,
          "Total Carp Inches": null,
          "Team Carp Inches": null,
          Picture: "https://i.imgur.com/kH3ovGv.jpg"
        },
        {
          Team: "Muchow-Marr",
          Competitor: "Muchow",
          Beat: "Alemeda -K",
          Species: "Carp",
          Time: [9, 11, 0, 0].join(":"),
          Length: 25.5,
          "Total Carp Inches": null,
          "Team Carp Inches": 25.5,
          Picture: "https://i.imgur.com/3tCGj1k.jpg"
        }
      ]
    }
  })
};
</script>
