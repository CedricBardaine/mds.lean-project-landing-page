<template>
  <v-app>
    <!-- <v-app-bar app color="black" dark dense
      >{{ $vuetify.breakpoint.name }} - dev</v-app-bar
    > -->

    <v-main>
      <div id="illu" class="red" style="height: 100vh">
        <v-row
          id="menu"
          class="green ma-0 pa-0"
          justify="center"
          style="height: 5%"
        >
          <v-row class="ma-0 pa-0 px-2 orange" align="center" justify="start">
            <span> Explor</span> <span class="indigo--text">'Area</span>
          </v-row>
          <v-row class="ma-0 pa-0 px-2" align="center" justify="end">
            <v-btn small text>A propos</v-btn>
            <v-btn small text>Contact</v-btn>
            <v-btn small fab color="white">
              <v-icon color="indigo"> mdi-plus </v-icon>
            </v-btn>
          </v-row>
        </v-row>

        <v-row
          id="content"
          class="yellow ma-0 pa-0"
          align="center"
          justify="center"
          style="height: 95%"
        >
          <v-row>
            <v-row class="col-12" justify="center">
              <span>
                Découvrez des lieux comme vous ne les avez jamais vus</span
              >
            </v-row>
            <v-row class="col-12" justify="center">
              <v-btn color="indigo" dark rounded> Accès anticipé </v-btn>
            </v-row>
          </v-row>
        </v-row>
      </div>

      <v-container>
        <v-skeleton-loader
          type="list-item-avatar-three-line, image, article, image, article, image, article"
        ></v-skeleton-loader>
      </v-container>
      <div>
        var de dev lisez pas :
        <span class="red white--text px-2">
        ({{$vuetify.breakpoint.name}})

        </span>
      </div>
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
