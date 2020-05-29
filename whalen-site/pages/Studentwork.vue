<template>
  <v-app>
    <div>
      <V-container>
        <v-row>
          <v-hover v-slot:default="{ hover }">
            <v-col id="loop" class="cols" cols="12" md="6">
              <v-expand-transition>
                <div
                  v-if="hover"
                  class="d-flex transition-fast-in-fast-out purple darken-2 v-card--reveal white--text flex-column"
                  style="height: 100%;"
                >
                  "Loop" By Class of 2020
                  <nuxt-link class="nuxt-link" to="/loop"
                    ><v-btn class="btn" active-class="no-active"
                      >Learn More</v-btn
                    ></nuxt-link
                  >
                </div>
              </v-expand-transition>
            </v-col>
          </v-hover>

          <v-spacer></v-spacer>
          <v-hover v-slot:default="{ hover }">
            <v-col id="jang" class="cols" cols="12" md="6">
              <v-expand-transition>
                <div
                  v-if="hover"
                  class="d-flex transition-fast-in-fast-out v-card--reveal green darken-2 v-card white--text flex-column"
                  style="height: 100%;"
                >
                  "Jang Foods" By Class of 2020
                  <nuxt-link class="nuxt-link" to="/jang"
                    ><v-btn class="btn" active-class="no-active"
                      >Learn More</v-btn
                    ></nuxt-link
                  >
                </div>
              </v-expand-transition>
            </v-col>
          </v-hover>
          <v-spacer></v-spacer>
          <v-hover v-slot:default="{ hover }">
            <v-col id="will" class="cols" cols="12">
              <v-expand-transition>
                <div
                  v-if="hover"
                  class="d-flex transition-fast-in-fast-out blue darken-2 v-card--reveal white--text flex-column"
                  style="height: 100%;"
                >
                  "Fire Emblem" By Class of 2020
                  <nuxt-link class="nuxt-link" to="/fireemblem"
                    ><v-btn class="btn" active-class="no-active"
                      >Learn More</v-btn
                    ></nuxt-link
                  >
                </div>
              </v-expand-transition>
            </v-col>
          </v-hover>
        </v-row>
        <StudentRowTwo />
        <v-lazy v-model="isActive">
          <StudentRowThree />
        </v-lazy>
      </V-container>
    </div>
  </v-app>
</template>

<script>
import "../assets/_StudentRows.scss";

import StudentRowTwo from "@/components/StudentRowTwo";
import StudentRowThree from "@/components/StudentRowThree";

export default {
  components: {
    StudentRowTwo,
    StudentRowThree
  },
  data() {
    return {
      hover: false,
      isActive: false
    };
  }
};
</script>

<style lang="scss" scoped></style>
