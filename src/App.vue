<template>
  <v-app>
    <v-main>
      <div class="scroller" ref="scrollSections">
        <!-- DIV : HERO  -->
        <nav class="menu">
          <div class="menu-left">
            <span> Explor'Area</span>
          </div>
          <div class="menu-right">
            <a href="/about">A propos</a>
            <a href="/contact">Contact</a>
            <v-btn small fab color="white">
              <v-icon color="indigo"> mdi-magnify </v-icon>
            </v-btn>
          </div>
        </nav>
        <section data-scroll-section id="idHero" class="section section-hero">
          <div data-scroll data-scroll-speed="1" class="section-content">
            <h1>
              Découvrez les villes<br />
              avec notre exploration<br />
              game phygital
            </h1>
            <a href="/" class="button-main">S'inscrire</a>
          </div>
          <img
            class="image-hero parallax-1"
            src="./assets/img/Foreground-1.png"
            alt=""
            data-scroll
            data-scroll-speed="2"
          />
          <img
            class="image-hero parallax-2"
            src="./assets/img/Background-1.png"
            alt=""
            data-scroll
            data-scroll-speed="1"
          />
        </section>

        <!-- end -->

        <!-- DIV : WHAT IS IT  -->

        <section class="section section-what" data-scroll-section>
          <div class="section-content">
            <img
              data-scroll
              data-scroll-speed="1"
              src="./assets/img/aie aie aie 1.png"
              alt=""
            />
            <div class="text-group">
              <h2>
                Découvrez des villes en toute autonomie grâce à nos scénarios
                interactifs guidés par application mobile
              </h2>
              <p>
                Il y a des lieux dans lesquels vous passez tous les jours. Il y
                en a d’autres que vous voulez découvrir. Dans les deux cas, il y
                a Explor’Area. Vivez une aventure immersive et dépaysante en
                explorant la ville de votre choix. Au moment que vous voulez,
                vous sélectionnez un des scénarios disponible localement et
                l’application vous lance dans l’histoire. Au fil des épreuves et
                des pièges vous explorez la ville, découvrez ses secrets, tout
                en vous amusant.
              </p>
            </div>
          </div>
        </section>

        <!-- end -->

        <!-- DIV : AVANTAGES -->

        <section
          id="idAvantages"
          no-gutters
          align="center"
          justify="center"
          class="section section-advantages"
          data-scroll-section
        >
          <div class="section-content">
            <CardAvantage
              icon="mdi-magnify"
              title="Des codes à débloquer"
              content="
                Progressez dans la ville en décryptant les codes qui vous
                dévoileront de nouveaux indices.
              "
              data-scroll
              data-scroll-speed="1"
            />

            <CardAvantage
              icon="mdi-lightbulb-on"
              title="Des énigmes à résoudre"
              content="Avancez de site en site en triomphant des pièges tendus par l’histoire que vous vivez"
              data-scroll
              data-scroll-speed="4"
            />

            <CardAvantage
              icon="mdi-magnify"
              title="Des indices à trouver sur les lieux"
              content="Tout au long de votre parcours, ayez l’oeil bien ouvert car des indices se cachent autour de vous"
              data-scroll
              data-scroll-speed="3"
            />
          </div>
        </section>

        <!-- end -->

        <!-- DIV : VIDEO -->

        <section
          class="section section-video custom-videoDiv"
          data-scroll-section
        >
          <div class="section-content">
            <h3>Découvrez les<br />prémices d’Explor’Area</h3>
            <div class="play-button">
              <img src="./assets/img/play.svg" alt="" />
            </div>
            <a href="/" class="button-main">S'inscrire</a>
          </div>
          <img
            src="./assets/img/anatoliy-gromov-o7fpEKG6W6U-unsplash_1.png"
            class="img-bg"
            data-scroll
            data-scroll-speed="1"
          />
        </section>

        <!-- end -->

        <!-- DIV : TESTIMONIALS -->

        <section class="section section-testimonials" data-scroll-section>
          <h2>
            Ils ont testé, ils ont aimé
          </h2>
        </section>

        <!-- end -->

        <!-- DIV : rien c'est pour le dev -->

        <div>
          var de dev lisez pas :
          <span class="red white--text px-2">
            ({{ $vuetify.breakpoint.name }})
          </span>
        </div>

        <!-- end -->
      </div>
    </v-main>
  </v-app>
</template>

<script>
import './assets/css/locomotive-scroll.css';
import './assets/css/css.css';
import locomotiveScroll from 'locomotive-scroll';
import CardAvantage from './components/CardAvantage';

export default {
  name: 'App',

  components: { CardAvantage },

  data() {
    return {
      scrollIns: null
    };
  },

  mounted() {
    const _self = this;
    this.$nextTick(() => {
      _self.initLocoScroll();
    });
  },

  methods: {
    initLocoScroll() {
      const _self = this;
      this.scroll = new locomotiveScroll({
        el: _self.$refs['scrollSections'],
        smooth: true,
        lerp: 0.1
      });
    }
  }
};
</script>
