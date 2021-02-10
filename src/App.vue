<template>
  <v-app>
    <!-- <v-app-bar app color="black" dark dense
      >{{ $vuetify.breakpoint.name }} - dev</v-app-bar
    > -->

    <v-main>
      <!-- DIV : HERO  -->

      <div id="idHero" style="height: 100vh">
        <v-row
          id="idMenu"
          class="ma-0 pa-0"
          justify="center"
          style="height: 5%"
        >
          <v-row class="ma-0 pa-0 px-2" align="center" justify="start">
            <span> Explor</span> <span class="indigo--text">'Area</span>
          </v-row>
          <v-row class="ma-0 pa-0 px-2" align="center" justify="end">
            <v-btn small text>A propos</v-btn>
            <v-btn small text>Contact</v-btn>
            <v-btn small fab color="white">
              <v-icon color="indigo"> mdi-magnify </v-icon>
            </v-btn>
          </v-row>
        </v-row>

        <v-row
          id="idHero-content"
          class="yellow ma-0 pa-0"
          align="center"
          justify="center"
          style="height: 95%"
        >
          <v-row>
            <v-row class="col-12 mx-4" justify="start">
              <span class="custom-mainTitle">
                Découvrez les villes avec notre exploration game phygital</span
              >
            </v-row>
            <v-row class="col-12 mx-4" justify="start">
              <v-btn class="custom-mainBtnText" color="indigo" dark rounded>
                Télécharger l’application
              </v-btn>
            </v-row>
          </v-row>
        </v-row>
      </div>

      <!-- end -->

      <!-- DIV : WHAT IS IT  -->

      <div
        id="idWhatIsIt"
        style="background-color: #5139ea; color: white; height: 100vh"
      >
        <v-container style="max-width: 830px">
          <v-row class="ma-0 pa-0 text-center" align="center" justify="center">
            <h2>
              Duis velit laborum mollit exercitation qui exercitation ea quis
              nulla laborum tempor id.
            </h2>

            <p>
              Excepteur reprehenderit commodo non minim veniam occaecat. Sint
              voluptate excepteur amet excepteur ullamco. Lorem eiusmod deserunt
              ex cupidatat laboris ipsum cillum deserunt.
            </p>
            <v-img src="./assets/img/aie aie aie 1.png"> </v-img>
          </v-row>
        </v-container>
      </div>

      <!-- end -->

      <!-- DIV : rien c'est pour le dev -->

      <div>
        var de dev lisez pas :
        <span class="red white--text px-2">
          ({{ $vuetify.breakpoint.name }})
        </span>
      </div>

      <!-- end -->
    </v-main>
  </v-app>
</template>

<script>
export default {
  name: "App",

  components: {},

  data: () => ({
    //
  }),
};
</script>

<style >
.custom-mainTitle {
  /* font-family: Averta CY; */
  font-size: 105px;
  font-weight: 600;
}
.custom-mainBtnText {
  font-size: 18px;
  font-weight: 600;
}
</style>
