<template>
  <div class="text-center">
    <h2>Loop</h2>
    <v-container>
      <v-row class="row">
        <v-col cols="12" md="6" class="text-center">
          <img class="mockup" src="../assets/loop/mock4.jpg" alt />
        </v-col>
        <v-col cols="12" class="text-center">
          <v-card class="text-center">
            <sub-header>Created By</sub-header>
            <v-divider></v-divider>
            <v-list>
              <li>
                Nick Melkadze
                <span class="span">CUNY Hunter 2024</span>
              </li>
              <li>
                Edward Ng
                <span class="span">Stony Brook University 2024</span>
              </li>
              <li>
                Veda Balte
                <span class="span">Cornell University 2024</span>
              </li>
              <li>
                Brendan Gallo
                <span class="span">RIT 2024</span>
              </li>
              <li>
                Thami Hamzane
                <span class="span">SITHS 2021</span>
              </li>
              <li>
                Ilsa Lareb
                <span class="span">SITHS 2021</span>
              </li>
            </v-list>
            <v-card-text>
              Loop is a Full-stack planner application built wtih NodeJS and
              Mongoose
            </v-card-text>

            <v-card-actions>
              <v-spacer></v-spacer>
              <v-btn
                text
                color="deep-purple accent-4"
                active-class="no-active"
                @click="onClickSite()"
              >Visit</v-btn>
              <v-btn @click="onClickGit()" text color="deep-purple accent-4">Github</v-btn>
              <v-spacer></v-spacer>
            </v-card-actions>
          </v-card>
        </v-col>
      </v-row>
      <v-row class="row">
        <v-col cols="12" md="4">
          <img class="mockup" src="../assets/loop/mock5-sm-min.jpg" alt />
        </v-col>
      </v-row>
    </v-container>
  </div>
</template>

<script>
export default {
  methods: {
    onClickSite: function() {
      window.open("https://www.planwithloop.com/auth/login", "_blank");
    },
    onClickGit: function() {
      window.open("https://github.com/melkadze/class-planner", "_blank");
    }
  }
};
</script>

<style lang="scss" scoped>
h2 {
  color: black;
  display: inline-block;
  border-bottom: 2px solid #aa00ff;
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
  color: #aa00ff;
}
</style>
