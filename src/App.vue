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

      <div class="red" style="height: 12px"></div>

    <img width="25%" style="height: 200px" src="./assets/logo.png">

<Helloscroll/>

      <div class="red" style="height: 12px"></div>

      <div>
        var de dev lisez pas :
        <span class="red white--text px-2">
          ({{ $vuetify.breakpoint.name }})
        </span>
      </div>
    </v-main>
  </v-app>
</template>

<script>
// import LocomotiveScroll from "locomotive-scroll";
import "./assets/css/locomotive-scroll.css";

import Helloscroll from "./components/Helloscroll";

export default {
  name: "App",

  components: {Helloscroll,},

  data: () => ({
    //
  }),
  mounted() {
  },
};
</script>

<style>
body {
  margin: 0;
  padding: 0;
  font-family: "Quicksand", sans-serif;
  color: #010101;
}
h4,
h1 {
  text-align: center;
}
h4 {
  font-weight: 600;
  font-size: 2em;
  margin-bottom: 0;
}
h1 {
  font-weight: 300;
  font-size: 4em;
  margin: 0;
}
.container {
  display: flex;
  width: 100%;
  height: 58vh;
  margin-top: 19em;
}
.getting-started {
  background-color: #e8e5e6;
  width: 30%;
  padding: 3em;
}
.getting-started h4 {
  text-align: left;
}
.getting-started p {
  font-size: 1.5em;
}
button {
  padding: 1.4em;
  width: 40%;
  background-color: #010101;
  color: #ffffff;
  border: none;
  outline: none;
}

.image-holder {
  width: 70%;
}
img {
  width: 100%;
  height: 100%;
  object-fit: cover;
  object-position: 50% 50%;
}
.gallery {
  padding: 2em;
  height: 200vh;
}
.image-pop {
  width: 20%;
  height: 30vh;
  position: relative;
}
#one {
  top: 3em;
  left: 5em;
}
#two {
  top: 4em;
  left: 60%;
}
#three {
  top: 8em;
  left: 10%;
}
#four {
  top: 3em;
  left: 70%;
}
#five {
  top: 6em;
  left: 30%;
}
</style>
