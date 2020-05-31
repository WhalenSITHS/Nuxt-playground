<template>
  <div>
    <v-row>
      <v-hover v-slot:default="{ hover }">
        <v-col data-aos="fade-right" id="choi" class="cols" cols="12" md="4">
          <v-expand-transition>
            <div
              v-if="hover"
              class="d-flex transition-fast-in-fast-out red darken-2 v-card--reveal white--text flex-column"
              style="height: 100%;"
            >
              <span class="SR2-Text">"East Harbor" By Karen Choi Class of 2021</span>
              <nuxt-link class="nuxt-link" to="/Eastharbor">
                <v-btn class="btn" active-class="no-active">Learn More</v-btn>
              </nuxt-link>
            </div>
          </v-expand-transition>
        </v-col>
      </v-hover>

      <v-spacer></v-spacer>
      <v-hover v-slot:default="{ hover }">
        <v-col data-aos="fade-down" id="poker" class="cols" cols="12" md="4">
          <v-expand-transition>
            <div
              v-if="hover"
              class="d-flex transition-fast-in-fast-out v-card--reveal green darken-2 v-card white--text flex-column"
              style="height: 100%;"
            >
              <span class="SR2-Text">"Black Jack" By Nick Melkadze Class of 2020</span>
              <nuxt-link class="nuxt-link" to="/fireemblem">
                <v-btn class="btn" active-class="no-active">Learn More</v-btn>
              </nuxt-link>
            </div>
          </v-expand-transition>
        </v-col>
      </v-hover>
      <v-spacer></v-spacer>
      <v-hover v-slot:default="{ hover }">
        <v-col data-aos="fade-left" id="yu" class="cols" cols="12" md="4">
          <v-expand-transition>
            <div
              v-if="hover"
              class="d-flex transition-fast-in-fast-out blue darken-2 v-card--reveal white--text flex-column"
              style="height: 100%;"
            >
              <span class="SR2-Text">"Cyberpunk Tokyo" By Kelly Yu Class of 2021</span>
              <nuxt-link class="nuxt-link" to="/fireemblem">
                <v-btn class="btn" active-class="no-active">Learn More</v-btn>
              </nuxt-link>
            </div>
          </v-expand-transition>
        </v-col>
      </v-hover>
    </v-row>
  </div>
</template>

<script>
import "../assets/_StudentRows.scss";
export default {
  name: "StudentRowTwo"
};
</script>

<style lang="scss" scoped></style>
