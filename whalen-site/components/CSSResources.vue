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
          <v-card-text
            class="card-text"
          >Flexbox is an incredible tool for modern web design. This resource will assist with the various flex properties</v-card-text>
          <v-btn @click="onClickFlexCheat()" text color="#03A9F4">Check It Out</v-btn>
        </v-card>
      </v-col>

      <v-col cols="12" md="3">
        <v-card raised class="d-inline-block mx-auto custom-card">
          <img class="card-logo" src="../assets/logos/tutplus.png" />
          <v-card-title class="font-weight-light">30 CSS Selectors</v-card-title>
          <v-card-text
            class="card-text"
          >This a great resource of various CSS selectors that you may find sueful in a pinch</v-card-text>
          <v-btn @click="onClickTutplus()" text color="#03A9F4">Visit</v-btn>
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
.custom-card {
  margin: 2rem 1rem auto;
  text-align: center;
  padding: 1rem;
  width: 100%;
  height: 20rem;
}
.row {
  margin: 6rem auto;
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