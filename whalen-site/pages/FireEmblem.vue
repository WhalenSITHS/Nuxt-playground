<template>
  <div class="text-center">
    <h2>Fire Emblem</h2>
    <v-container>
      <v-row class="row">
        <v-col cols="12" md="6" class="text-center">
          <img class="mockup" src="../assets/Fire/mock1-min.jpg" alt />
        </v-col>
        <v-col cols="12" class="text-center">
          <v-card class="text-center">
            <sub-header>Created By</sub-header>
            <v-divider></v-divider>
            <v-list>
              <li>
                William Anderson
                <span class="span">CUNY Hunter 2024</span>
              </li>
              <li>
                Kai Tong Gao
                <span class="span">Cornell 2024</span>
              </li>
              <li>
                Sarah Abdel Fatah
                <span class="span">CUNY 2024</span>
              </li>
              <li>
                Winny Chan
                <span class="span">CUNY 2024</span>
              </li>
            </v-list>
            <v-card-text>Fire Emblem is a Full-stack online game based on the popular Fire Emblem franchise. The game is built using NodeJS, Socket.io and MongoDB</v-card-text>

            <v-card-actions>
              <v-spacer></v-spacer>
              <v-btn text color="blue accent-2" active-class="no-active" @click="onClickSite">Visit</v-btn>
              <v-btn @click="onClickGit" text color="blue accent-2">Github</v-btn>
              <v-spacer></v-spacer>
            </v-card-actions>
          </v-card>
        </v-col>
      </v-row>
      <v-row class="row">
        <v-col cols="12" md="4">
          <img class="mockup" src="../assets/Fire/mock2-min.jpg" alt />
        </v-col>
      </v-row>
    </v-container>
  </div>
</template>

<script>
export default {
  methods: {
    onClickGit() {
      location.href = `https://github.com/William-Anderson2020/Full-Stack-Project`;
    },
    onClickSite() {
      location.href = `https://full-stack-game.herokuapp.com/login`;
    }
  }
};
</script>

<style lang="scss" scoped>
h2 {
  color: black;
  display: inline-block;
  border-bottom: 2px solid #448aff;
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
  color: #448aff;
}
</style>
