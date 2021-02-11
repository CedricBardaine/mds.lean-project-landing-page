<template>
  <v-app>
    <!-- <v-app-bar app color="black" dark dense
      >{{ $vuetify.breakpoint.name }} - dev</v-app-bar
    > -->

    <v-main>
      <!-- DIV : HERO  -->

      <div id="idHero" style="height: 100vh">
        <v-row id="idMenu" no-gutters style="height: 5%">
          <v-row class="px-2" no-gutters align="center" justify="start">
            <span> Explor</span> <span class="indigo--text">'Area</span>
          </v-row>
          <v-row class="px-2" no-gutters align="center" justify="end">
            <v-btn small text>A propos</v-btn>
            <v-btn small text>Contact</v-btn>
            <v-btn small fab color="white">
              <v-icon color="indigo"> mdi-magnify </v-icon>
            </v-btn>
          </v-row>
        </v-row>

        <v-row
          id="idHero-content"
          class="yellow"
          no-gutters
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

      <v-row
        id="idWhatIsIt"
        no-gutters
        align="center"
        justify="center"
        style="background-color: #5139ea; color: white; height: 100vh"
      >
        <v-col class="" style="">
          <v-row>
            <v-row class="col-12 col-sm-6">
              <v-img src="./assets/img/aie aie aie 1.png"> </v-img>
            </v-row>
            <v-row class="col-12 col-sm-6">
              <v-row class="pb-4" align="end">
                <h2>
                  Découvrez des villes en toute autonomie grâce à nos scénarios
                  interactifs guidés par application mobile
                </h2>
              </v-row>

              <v-row class="pt-4" align="start">
                <p>
                  Il y a des lieux dans lesquels vous passez tous les jours. Il
                  y en a d’autres que vous voulez découvrir. Dans les deux cas,
                  il y a Explor’Area. Vivez une aventure immersive et dépaysante
                  en explorant la ville de votre choix. Au moment que vous
                  voulez, vous sélectionnez un des scénarios disponible
                  localement et l’application vous lance dans l’histoire. Au fil
                  des épreuves et des pièges vous explorez la ville, découvrez
                  ses secrets, tout en vous amusant.
                </p>
              </v-row>
            </v-row>
          </v-row>
        </v-col>
      </v-row>

      <!-- end -->

      <!-- DIV : AVANTAGES -->

      <v-row
        id="idAvantages"
        no-gutters
        align="center"
        justify="center"
        style="background-color: #ffffff; height: 100vh"
      >
        <v-container>
          <v-row justify="center" align="center">
            <v-row class="col-3 mx-2" align="end" style="height: 100%">
              <CardAvantage
                icon="mdi-magnify"
                title="Des codes à débloquer"
                content="
                Progressez dans la ville en décryptant les codes qui vous
                dévoileront de nouveaux indices.
              "
              />
              <v-spacer style="min-height: 192px"></v-spacer>
            </v-row>
            <v-row class="col-3 mx-2" align="start" style="height: 100%">
              <v-spacer style="min-height: 192px"></v-spacer>
              <CardAvantage
                icon="mdi-lightbulb-on"
                title="Des énigmes à résoudre"
                content="Avancez de site en site en triomphant des pièges tendus par l’histoire que vous vivez"
              />
            </v-row>
            <v-row class="col-3 mx-2" align="end" style="height: 100%">
              <CardAvantage
                icon="mdi-magnify"
                title="Des indices à trouver sur les lieux"
                content="Tout au long de votre parcours, ayez l’oeil bien ouvert car des indices se cachent autour de vous"
              />
              <v-spacer style="min-height: 192px"></v-spacer>
            </v-row>
          </v-row>
        </v-container>
      </v-row>

      <!-- end -->

      <!-- DIV : VIDEO -->

      <div class="custom-videoDiv" style="height: 100vh; position: relative">
        <h3
          style="
            position: absolute;
            color: white;
            padding-left: 80px;
            padding-top: 80px;
            font-size: 80px;
            width: 925px;
          "
        >
          Découvrez les prémices d’Explor’Area
        </h3>

        <v-row align="center" justify="center" style="height: 100%">
          <v-btn class="" fab style="height: 178px; width: 178px">
            <v-icon color="#5139ea" style="font-size: 133.5px">
              mdi-play
            </v-icon>
          </v-btn>
        </v-row>

        <v-btn
          class="custom-mainBtnText"
          rounded
          style="
            background-color: white;
            color: rgb(81, 57, 234);
            position: absolute;
            bottom: 108px;
            margin-left: 80px;
            height: 66px;
            font-size: 18px;
          "
        >
          Télécharger l’application
        </v-btn>
      </div>

      <!-- end -->

      <!-- DIV : TESTIMONIALS -->

      <div
        style="
          height: 100vh;
          background-color: #5139ea;
          color: white;
          position: relative;
        "
      >
        <h3
          style="
            position: absolute;
            color: white;
            left: 178px;
            top: 113px;
            font-size: 80px;
            width: 531px;
          "
        >
          Ils ont testé, ils ont aimé
        </h3>

        <!-- TODO: faire la liste qui défile -->
        <v-row
          no-gutters
          style="
            position: absolute;
            bottom: 211px;
            left: 277px;
            flex-wrap: nowrap;
          "
        >
          <CardTestimonials
            img="https://raw.githubusercontent.com/ArjunAtlast/Profile-Card/master/assets/john-doe.png"
          />
          <CardTestimonials />
          <CardTestimonials />
          <CardTestimonials />
          <CardTestimonials />
          <CardTestimonials />
        </v-row>
      </div>

      <!-- end -->

      <!-- DIV : FAQ -->

      <div style="height: 100vh; background-color: white">
        <v-row justify="center" style="margin: 80px 80px">
          <h3>Questions fréquentes</h3>
        </v-row>
        <v-row justify="center">
          <v-container>
            <v-expansion-panels inset>
              <v-expansion-panel>
                <v-expansion-panel-header disable-icon-rotate>
                  Qu’est-ce qu’un Exploration Game ?
                  <template v-slot:actions>
                    <v-btn x-small color="#5139ea" fab elevation="0">
                      <v-icon color="white"> mdi-plus </v-icon>
                    </v-btn>
                  </template>
                </v-expansion-panel-header>
                <v-expansion-panel-content>
                  Lorem ipsum dolor sit amet, consectetur adipiscing elit, sed
                  do eiusmod tempor incididunt ut labore et dolore magna aliqua.
                  Ut enim ad minim veniam, quis nostrud exercitation ullamco
                  laboris nisi ut aliquip ex ea commodo consequat.
                </v-expansion-panel-content>
              </v-expansion-panel>
              <v-expansion-panel>
                <v-expansion-panel-header disable-icon-rotate>
                  Qu'est ce qu'un jeu phygital ?
                  <template v-slot:actions>
                    <v-btn x-small color="#5139ea" fab elevation="0">
                      <v-icon color="white"> mdi-plus </v-icon>
                    </v-btn>
                  </template>
                </v-expansion-panel-header>
                <v-expansion-panel-content>
                  Lorem ipsum dolor sit amet, consectetur adipiscing elit, sed
                  do eiusmod tempor incididunt ut labore et dolore magna aliqua.
                  Ut enim ad minim veniam, quis nostrud exercitation ullamco
                  laboris nisi ut aliquip ex ea commodo consequat.
                </v-expansion-panel-content>
              </v-expansion-panel>
              <v-expansion-panel>
                <v-expansion-panel-header disable-icon-rotate>
                  A combien peut-on jouer à un scénario Explor’Area ?
                  <template v-slot:actions>
                    <v-btn x-small color="#5139ea" fab elevation="0">
                      <v-icon color="white"> mdi-plus </v-icon>
                    </v-btn>
                  </template>
                </v-expansion-panel-header>
                <v-expansion-panel-content>
                  Lorem ipsum dolor sit amet, consectetur adipiscing elit, sed
                  do eiusmod tempor incididunt ut labore et dolore magna aliqua.
                  Ut enim ad minim veniam, quis nostrud exercitation ullamco
                  laboris nisi ut aliquip ex ea commodo consequat.
                </v-expansion-panel-content>
              </v-expansion-panel>
              <v-expansion-panel>
                <v-expansion-panel-header disable-icon-rotate>
                  Quel est le niveau de difficulté du jeu ?
                  <template v-slot:actions>
                    <v-btn x-small color="#5139ea" fab elevation="0">
                      <v-icon color="white"> mdi-plus </v-icon>
                    </v-btn>
                  </template>
                </v-expansion-panel-header>
                <v-expansion-panel-content>
                  Lorem ipsum dolor sit amet, consectetur adipiscing elit, sed
                  do eiusmod tempor incididunt ut labore et dolore magna aliqua.
                  Ut enim ad minim veniam, quis nostrud exercitation ullamco
                  laboris nisi ut aliquip ex ea commodo consequat.
                </v-expansion-panel-content>
              </v-expansion-panel>
              <v-expansion-panel>
                <v-expansion-panel-header disable-icon-rotate>
                  Peut-on rejouer un de vos scénarios ?
                  <template v-slot:actions>
                    <v-btn x-small color="#5139ea" fab elevation="0">
                      <v-icon color="white"> mdi-plus </v-icon>
                    </v-btn>
                  </template>
                </v-expansion-panel-header>
                <v-expansion-panel-content>
                  Lorem ipsum dolor sit amet, consectetur adipiscing elit, sed
                  do eiusmod tempor incididunt ut labore et dolore magna aliqua.
                  Ut enim ad minim veniam, quis nostrud exercitation ullamco
                  laboris nisi ut aliquip ex ea commodo consequat.
                </v-expansion-panel-content>
              </v-expansion-panel>
              <v-expansion-panel>
                <v-expansion-panel-header disable-icon-rotate>
                  Dans quelle ville puis-je jouer à Explor’Area ?
                  <template v-slot:actions>
                    <v-btn x-small color="#5139ea" fab elevation="0">
                      <v-icon color="white"> mdi-plus </v-icon>
                    </v-btn>
                  </template>
                </v-expansion-panel-header>
                <v-expansion-panel-content>
                  Lorem ipsum dolor sit amet, consectetur adipiscing elit, sed
                  do eiusmod tempor incididunt ut labore et dolore magna aliqua.
                  Ut enim ad minim veniam, quis nostrud exercitation ullamco
                  laboris nisi ut aliquip ex ea commodo consequat.
                </v-expansion-panel-content>
              </v-expansion-panel>
            </v-expansion-panels>
          </v-container>
        </v-row>
      </div>

      <!-- end -->

      <!-- DIV : Footer -->

      <v-row
        style="background-color: #5139ea; color: white; min-height: 12px"
        no-gutters
      >
        <v-row
          class="col-3"
          no-gutters
          justify="center"
          style="margin-top: 142px"
          >Explor'Area</v-row
        >
        <v-row
          class="col-6"
          style="margin-top: 202px"
          no-gutters
          justify="center"
          align="center"
        >
          <v-row no-gutters>
            <p style="width: 66%">
              Explor’Area est un projet développé dans le cadre des Master de
              l’éroce My Digital School Rennes.
            </p>
          </v-row>
          <v-row no-gutters>
            <v-row no-gutters class="col-4 ma-0 pa-2" align="center"
              >Home <br />
              About <br />
              Contact</v-row
            >
            <v-row no-gutters class="col-4 ma-0 pa-2" align="center"
              >CGU <br />
              CGV <br />
              Mentions légales</v-row
            >
            <v-row no-gutters class="col-4 ma-0 pa-2" align="center">
              <v-row no-gutters class="col-12"> Suivez nous </v-row>
              <v-row no-gutters class="col-12">
                <v-icon color="white" class="mr-4">mdi-facebook</v-icon>
                <v-icon color="white" class="mr-4">mdi-instagram</v-icon>
                <v-icon color="white" class="mr-4">mdi-twitter</v-icon>
              </v-row>
            </v-row>
            <small style="margin: 124px 0px 32px 0px; font-size: 11px"
              >Concepteurs et propriétaires : Cédric Bardaine, Florian Calvo,
              Manon Cauque, Yaneck Chareyre, Gloria Chesnel et Sébastien
              Degrange</small
            >
          </v-row>
        </v-row>
        <v-row
          class="col-3"
          style="margin-top: 124px"
          no-gutters
          justify="center"
        >
          <v-btn color="white" fab @click="smoothScrollToTop()">
            <v-icon color="#5139ea">mdi-arrow-up</v-icon>
          </v-btn>
        </v-row>
      </v-row>

      <!-- end -->
    </v-main>
  </v-app>
</template>

<script>
import "./assets/css/css.css";

import CardAvantage from "./components/CardAvantage";
import CardTestimonials from "./components/CardTestimonials";

export default {
  name: "App",

  components: { CardAvantage, CardTestimonials },

  data: () => ({
    //
  }),
  methods: {
    smoothScrollToTop() {
      window.scrollTo({ top: 0, behavior: "smooth" });
    },
  },
};
</script>
