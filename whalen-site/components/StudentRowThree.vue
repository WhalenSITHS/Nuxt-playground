<template>
  <div>
    <v-row>
      <v-hover v-slot:default="{ hover }">
        <v-col data-aos="flip-up" id="pkmn" class="cols" cols="12">
          <v-expand-transition>
            <div
              v-if="hover"
              class="d-flex transition-fast-in-fast-out orange darken-2 v-card--reveal white--text flex-column"
              style="height: 100%;"
            >
              'Pokemon Duel' By William Anderson Class of 2020
              <nuxt-link class="nuxt-link" to="/Pokemon">
                <v-btn class="btn" active-class="no-active">Learn More</v-btn>
              </nuxt-link>
            </div>
          </v-expand-transition>
        </v-col>
      </v-hover>

      <v-spacer></v-spacer>
      <v-hover v-slot:default="{ hover }">
        <v-col data-aos="flip-right" id="kai" class="cols" cols="12" md="6">
          <v-expand-transition>
            <div
              v-if="hover"
              class="d-flex transition-fast-in-fast-out v-card--reveal green darken-2 v-card white--text flex-column"
              style="height: 100%;"
            >
              <span class="SR3">"Kai's Forest Blog" By Kai Tong Gao Class of 2020</span>
              <nuxt-link class="nuxt-link" to="/Whatliesbelow">
                <v-btn class="btn" active-class="no-active">Learn More</v-btn>
              </nuxt-link>
            </div>
          </v-expand-transition>
        </v-col>
      </v-hover>
      <v-spacer></v-spacer>
      <v-hover v-slot:default="{ hover }">
        <v-col data-aos="flip-left" id="bao" class="cols" cols="12" md="6">
          <v-expand-transition>
            <div
              v-if="hover"
              class="d-flex transition-fast-in-fast-out pink darken-2 v-card--reveal white--text flex-column"
              style="height: 100%;"
            >
              <span class="SR3">"Japan" By Bao Bao Chen Class of 2021</span>
              <nuxt-link class="nuxt-link" to="/Japan">
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
export default {};
</script>

<style lang="scss" scoped></style>
