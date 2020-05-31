<template>
  <div class="text-center">
    <h2>Jang Foods</h2>
    <v-container>
      <v-row class="row">
        <v-col cols="12" md="6" class="text-center">
          <img class="mockup" src="../assets/Jang/mock3-min.jpg" alt />
        </v-col>
        <v-col cols="12" class="text-center">
          <v-card class="text-center">
            <sub-header>Created By</sub-header>
            <v-divider></v-divider>
            <v-list>
              <li>
                Carlo Dugo
                <span class="span">Northeastern 2024</span>
              </li>
              <li>
                Dejon Kurti
                <span class="span">MIT 2024</span>
              </li>
              <li>
                Bryan Boyd
                <span class="span">Princeton 2024</span>
              </li>
              <li>
                Cornelia Murja
                <span class="span">Macaulay Baruch 2024</span>
              </li>
              <li>
                Brian Jiang
                <span class="span">Northeastern 2024</span>
              </li>
              <li>
                Andrew Bishay
                <span class="span">SITHS 2021</span>
              </li>
            </v-list>
            <v-card-text>Jang Foods is a full-stack online food service application. Jang foods is powered by NodeJS, MongoDB and the Stripe API</v-card-text>

            <v-card-actions>
              <v-spacer></v-spacer>
              <v-btn
                text
                color="light-green darken-4"
                active-class="no-active"
                @click="onClickSite"
              >Visit</v-btn>
              <v-btn @click="onClickGit" text color="light-green darken-4">Github</v-btn>
              <v-spacer></v-spacer>
            </v-card-actions>
          </v-card>
        </v-col>
      </v-row>
      <v-row class="row">
        <v-col cols="12" md="4">
          <img class="mockup" src="../assets/Jang/mock2-min.jpg" alt />
        </v-col>
      </v-row>
    </v-container>
  </div>
</template>

<script>
export default {
  methods: {
    onClickGit() {
      location.href = `https://github.com/cdugo/jang-foodcart`;
    },
    onClickSite() {
      location.href = `https://jang-food.herokuapp.com/`;
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
  margin: 6rem 1rem auto;
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
</style>
