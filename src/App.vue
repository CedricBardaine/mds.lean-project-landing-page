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
              style="height: fit-content; width: -webkit-fill-available"
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
            data-scroll-speed="2"
          />
        </section>

        <!-- end -->

        <!-- DIV : TESTIMONIALS -->

        <section class="section section-testimonials" data-scroll-section>
          <div class="section-content">
            <h2>
              Ils ont testé,<br />
              ils ont aimé
            </h2>
            <div id="direction">
              <div
                class="cards-container"
                data-scroll
                data-scroll-direction="horizontal"
                data-scroll-target="#direction"
                data-scroll-speed="5"
              >
                <CardTestimonial />
                <CardTestimonial />
                <CardTestimonial />
                <CardTestimonial />
                <CardTestimonial />
                <CardTestimonial />
                <CardTestimonial />
                <CardTestimonial />
              </div>
            </div>
          </div>
        </section>

        <!-- end -->

        <section class="section section-faq" data-scroll-section>
          <div class="section-content">
            <h2>
              Questions<br />
              fréquentes
            </h2>
            <div class="faq-container">
              <div class="faq-question-upper">
                <div class="q-title">Qu'est-ce qu'un exploration game ?</div>
                <img src="./assets/img/plus-button.svg" alt="" />
              </div>
              <div class="faq-question-line"></div>
            </div>
            <div class="faq-container">
              <div class="faq-question-upper">
                <div class="q-title">Qu’est-ce qu’un jeu phygital ?</div>
                <img src="./assets/img/plus-button.svg" alt="" />
              </div>
              <div class="faq-question-line"></div>
            </div>
            <div class="faq-container">
              <div class="faq-question-upper">
                <div class="q-title">
                  A combien peut-on jouer à un scénario Explor’Area ?
                </div>
                <img src="./assets/img/plus-button.svg" alt="" />
              </div>
              <div class="faq-question-line"></div>
            </div>
            <div class="faq-container">
              <div class="faq-question-upper">
                <div class="q-title">
                  Quel est le niveau de difficulté du jeu ?
                </div>
                <img src="./assets/img/plus-button.svg" alt="" />
              </div>
              <div class="faq-question-line"></div>
            </div>
            <div class="faq-container">
              <div class="faq-question-upper">
                <div class="q-title">Peut-on rejouer un de vos scénarios ?</div>
                <img src="./assets/img/plus-button.svg" alt="" />
              </div>
              <div class="faq-question-line"></div>
            </div>
            <div class="faq-container">
              <div class="faq-question-upper">
                <div class="q-title">
                  Dans quelle ville puis-je jouer à Explor’Area ?
                </div>
                <img src="./assets/img/plus-button.svg" alt="" />
              </div>
              <div class="faq-question-line"></div>
            </div>
          </div>
        </section>
        <section class="section section-pre-footer" data-scroll-section>
          <img src="./assets/img/illu-pre-footer.png" alt="" />
          <div class="pre-footer-content">
            <h2>Accédez à notre application</h2>
            <a href="#" class="button-main">S'inscrire</a>
          </div>
        </section>
        <section class="footer" data-scroll-section>
          <div class="section-content">
            <h4 class="logo">Explor'Area</h4>
            <div class="footer-inner">
              <div class="desc">
                Explor’Area est un projet développé dans le cadre<br />
                des Master de l’école My Digital School Rennes.
              </div>
              <div class="list">
                <div class="col">
                  <a href="" class="f-link">Home</a>
                  <a href="" class="f-link">About</a>
                  <a href="" class="f-link">Contact</a>
                </div>
                <div class="col">
                  <a href="" class="f-link">CGU</a>
                  <a href="" class="f-link">CGV</a>
                  <a href="" class="f-link">Mentions légales</a>
                </div>
                <div class="col">
                  <p href="" class="f-link">Suivez-nous</p>
                  <div class="socials">
                    <a href="" class="social-link"
                      ><img src="./assets/img/facebook-f.svg"
                    /></a>
                    <a href="" class="social-link">
                      <img src="./assets/img/twitter-alt.svg" />
                    </a>
                    <a href="" class="social-link">
                      <img src="./assets/img/instagram.svg" />
                    </a>
                  </div>
                </div>
              </div>
              <div class="copyright">
                Concepteurs et propriétaires : Cédric Bardaine, Florian Cario,
                Manon Cauque, Yaneck Chareyre, Gloria Chesnel et Sébastien
                Degrange
              </div>
            </div>
          </div>
        </section>
      </div>
    </v-main>
  </v-app>
</template>

<script>
import './assets/css/locomotive-scroll.css';
import './assets/css/css.css';
import locomotiveScroll from 'locomotive-scroll';
import CardAvantage from './components/CardAvantage';
import CardTestimonial from './components/CardTestimonial';

export default {
  name: 'App',

  components: { CardAvantage, CardTestimonial },

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
