<template>
  <div>
    <v-row>
      <v-col cols="12">
        <h1>CSS/SCSS Resources</h1>
      </v-col>
      <v-col cols="12" md="3">
        <v-card raised class="d-inline-block mx-auto custom-card">
          <img class="card-logo" src="../assets/logos/mdn.svg" />
          <v-card-title class="font-weight-light">MDN</v-card-title>
          <v-card-text
            class="card-text"
          >MDN Should be your first stop to troubleshoot or look up CSS or JS information.</v-card-text>
          <v-btn @click="onClickMDN()" text color="#03A9F4">Check Them Out</v-btn>
        </v-card>
      </v-col>

      <v-col cols="12" md="3">
        <v-card raised class="d-inline-block mx-auto custom-card">
          <img class="card-logo" src="../assets/logos/flexbox-cheat.png" />
          <v-card-title class="font-weight-light">Flexbox Cheatsheat</v-card-title>
          <v-card-text class="card-text">This resource will assist with the various flex properties</v-card-text>
          <v-btn @click="onClickFlexCheat()" text color="#03A9F4">Check It Out</v-btn>
        </v-card>
      </v-col>

      <v-col cols="12" md="3">
        <v-card raised class="d-inline-block mx-auto custom-card">
          <img class="card-logo" src="../assets/logos/tutplus.png" />
          <v-card-title class="font-weight-light">30 CSS Selectors</v-card-title>
          <v-card-text
            class="card-text"
          >This a great resource of various CSS selectors that you may find useful in a pinch</v-card-text>
          <v-btn @click="onClickTutplus()" text color="#03A9F4">Visit</v-btn>
        </v-card>
      </v-col>
    </v-row>
    <v-row>
      <v-col cols="12" md="3">
        <v-card raised class="d-inline-block mx-auto custom-card">
          <img class="card-logo" src="../assets/logos/css-5.svg" />
          <v-card-title class="font-weight-light">Clippy</v-card-title>
          <v-card-text class="card-text">Easily create CSS clip paths with a handy GUI.</v-card-text>
          <v-btn @click="onClickClippy()" text color="#03A9F4">Check Them Out</v-btn>
        </v-card>
      </v-col>

      <v-col cols="12" md="3">
        <v-card raised class="d-inline-block mx-auto custom-card">
          <img class="card-logo" src="../assets/logos/html5.svg" />
          <v-card-title class="font-weight-light">Cubic Bezier</v-card-title>
          <v-card-text class="card-text">Cubic Bezier can help you nail down animation timings.</v-card-text>
          <v-btn @click="onClickCubicBezier()" text color="#03A9F4">Check It Out</v-btn>
        </v-card>
      </v-col>

      <v-col cols="12" md="3">
        <v-card raised class="d-inline-block mx-auto custom-card">
          <img class="card-logo" src="../assets/logos/Sass Logo (Color).png" />
          <v-card-title class="font-weight-light">
            SCSS
            <br />Documentation
          </v-card-title>
          <v-card-text class="card-text">Offical SCSS documentation for your referance.</v-card-text>
          <v-btn @click="onClickSCSS()" text color="#03A9F4">Visit</v-btn>
        </v-card>
      </v-col>
    </v-row>
    <v-row>
      <v-col cols="12" md="6">
        <v-card raised class="d-inline-block mx-auto custom-card">
          <img class="card-logo" src="../assets/logos/css-tricks.png" />
          <v-card-title class="font-weight-light">CSS Tricks</v-card-title>
          <v-card-text class="card-text">Great blog with amazing contributions for web development.</v-card-text>
          <v-btn @click="onClickCSSTricks()" text color="#03A9F4">Visit</v-btn>
        </v-card>
      </v-col>
    </v-row>
  </div>
</template>

<script>
export default {
  methods: {
    onClickMDN: function() {
      window.open(
        "https://developer.mozilla.org/en-US/docs/Web/CSS/Reference",
        "_blank"
      );
    },
    onClickFlexCheat: function() {
      window.open("https://yoksel.github.io/flex-cheatsheet/", "_blank");
    },
    onClickTutplus: function() {
      window.open(
        "https://code.tutsplus.com/tutorials/the-30-css-selectors-you-must-memorize--net-16048"
      );
    },
    onClickSCSS: function() {
      window.open("https://sass-lang.com/documentation");
    },
    onClickClippy: function() {
      window.open("https://bennettfeely.com/clippy/");
    },
    onClickCSSTricks: function() {
      window.open("https://css-tricks.com/");
    },
    onClickCubicBezier: function() {
      window.open("https://cubic-bezier.com/#.17,.67,.83,.67");
    }
  }
};
</script>

<style lang="scss" scoped>
div {
}
h1 {
  margin: 0.5rem auto;
  font-family: "Roboto", serif;
  text-transform: uppercase;
  text-align: center;
  color: #01579b;
}
.v-card__title {
  color: #03a9f4;
  margin: 5px auto;
  display: block;
}
@media screen and (max-width: 1264px) {
  .v-card__title {
    font-size: 1rem;
  }
}
.custom-card {
  margin: 2rem 1rem auto;
  text-align: center;
  padding: 1rem;
  width: 100%;
  height: 20rem;
  transition: 0.3s;
}
.custom-card:hover {
  transform: scale(1.1);
}
.row {
  margin: 1rem auto;
  padding: 3rem 0;
  width: 90vw;
  display: flex;
  justify-content: space-around;
  align-items: center;
}
.card-text {
  width: 80%;
  text-align: center;
  margin: 0 auto;
}
.card-logo {
  height: 3rem;
  margin: 3px auto;
}
</style>