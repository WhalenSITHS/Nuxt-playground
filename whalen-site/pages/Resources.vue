<template>
  <div>
    <v-row>
      <v-col cols="12">
        <h1>Development Environment</h1>
      </v-col>
      <v-col cols="12" md="3">
        <v-card raised class="d-inline-block mx-auto custom-card">
          <img class="card-logo" src="../assets/logos/VSCode.svg" />
          <v-card-title class="font-weight-light">VSCode Download</v-card-title>
          <v-card-text
            class="card-text"
          >VSCode is the only editor I use in class and it is recommended you use this.</v-card-text>
          <v-btn @click="onClickVSCode()" text color="#03A9F4">Download</v-btn>
        </v-card>
      </v-col>

      <v-col cols="12" md="3">
        <v-card raised class="d-inline-block mx-auto custom-card">
          <img class="card-logo" src="../assets/logos/visual-studio-2013.svg" />
          <v-card-title class="font-weight-light">My VSCode Settings</v-card-title>
          <v-card-text
            class="card-text"
          >This is a link to my VSCode settings. It is recommended you install my extensions and copy my settings.</v-card-text>
          <v-btn @click="onClickSettings()" text color="#03A9F4">Get My Settings</v-btn>
        </v-card>
      </v-col>

      <v-col cols="12" md="3">
        <v-card raised class="d-inline-block mx-auto custom-card">
          <img class="card-logo" src="../assets/logos/emmet.svg" />
          <v-card-title class="font-weight-light">Emmet Cheat Sheet</v-card-title>
          <v-card-text class="card-text">Check out this useful Emmet Cheat Sheet for VSCode</v-card-text>
          <v-btn @click="onClickEmmet()" text color="#03A9F4">Visit</v-btn>
        </v-card>
      </v-col>
    </v-row>
    <CSSResources />
  </div>
</template>

<script>
import CSSResources from "@/components/CSSResources";
export default {
  components: {
    CSSResources
  },
  methods: {
    onClickEmmet: function() {
      window.open("https://docs.emmet.io/cheat-sheet/", "_blank");
    },
    onClickVSCode: function() {
      window.open("https://code.visualstudio.com/download", "_blank");
    },
    onClickSettings: function() {
      window.open(
        "https://github.com/WhalenSITHS/Markdown-vscode/blob/master/vscode.md",
        "_blank"
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
  color: white;
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
}
.row {
  margin: 6rem auto;
  padding: 3rem 0;
  width: 90vw;
  display: flex;
  justify-content: space-around;
  align-items: center;
  background-color: #01579b;
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