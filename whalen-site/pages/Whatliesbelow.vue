<template>
  <div class="text-center">
    <h2>Kai's Forest Blog</h2>
    <v-container>
      <v-row class="row">
        <v-col cols="12" md="6" class="text-center">
          <img class="mockup" src="../assets/Kai/kaimock3-sm-min.jpg" alt />
        </v-col>
        <v-col cols="12" class="text-center">
          <v-card class="text-center">
            <sub-header>Created By</sub-header>
            <v-divider></v-divider>
            <v-list>
              <li>
                Kai Tong Gao
                <span class="span">Cornell 2024</span>
              </li>
            </v-list>
            <v-card-text
              class="card-text"
            >This project is is built on SCSS and HTML and is meant to gauge student mastery of industry standard HTML and CSS skills without leaning on JavaScript.</v-card-text>

            <v-card-actions>
              <v-spacer></v-spacer>
              <v-btn
                text
                color="light-green darken-4"
                active-class="no-active"
                @click="onClickSite()"
              >Visit</v-btn>
              <v-btn @click="onClickGit()" text color="light-green darken-4">Github</v-btn>
              <v-spacer></v-spacer>
            </v-card-actions>
          </v-card>
        </v-col>
      </v-row>
      <v-row class="row">
        <v-col cols="12" md="4">
          <img class="mockup" src="../assets/Kai/kaimock2-sm-min.jpg" alt />
        </v-col>
      </v-row>
    </v-container>
  </div>
</template>

<script>
export default {
  methods: {
    onClickSite: function() {
      window.open("https://kaisforestblog.netlify.app/", "_blank");
    },
    onClickGit: function() {
      window.open("https://github.com/kaitonggao/KaisForestBlog", "_blank");
    }
  }
};
</script>

<style lang="scss" scoped>
h2 {
  color: black;
  display: inline-block;
  border-bottom: 2px solid #33691e;
  font-size: 4rem;
  font-family: "Arvo", serif;
  text-transform: uppercase;
  margin: 6rem 2rem auto;
  text-align: center;
}
.row {
  margin: 3rem auto;
  justify-content: space-around;
  align-items: center;
}
.mockup {
  width: 100%;
}
.container {
  height: 95vh;
}
.v-card {
  padding: 1.5rem;
}
li {
  list-style: none;
  font-size: 1.2rem;
  margin: 1rem;
}
.span {
  font-style: italic;
  display: block;
  color: #33691e;
}
.card-text {
  width: 50%;
  text-align: center;
  margin: 0 auto;
}
@media screen and(max-width: 960px) {
  .card-text {
    width: 100%;
  }
  h2 {
    font-size: 2.5rem;
  }
}
</style>
