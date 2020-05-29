<template>
  <div>
    <v-container>
      <v-row class="pa-8 align">
        <v-col>
          <img
            data-aos="fade-right"
            src="../assets/logos/Sass Logo (Color).png"
          />
        </v-col>
        <v-col>
          <img data-aos="fade-up" src="../assets/logos/mongo.png" />
        </v-col>
        <v-col>
          <img data-aos="fade-left" src="../assets/logos/azure.png" />
        </v-col>
      </v-row>

      <v-row class="pa-8 align" v-lazy>
        <v-col>
          <img data-aos="fade-right" src="../assets/logos/Vuelogo.png" />
        </v-col>
        <v-col>
          <img data-aos="fade-up" src="../assets/logos/firebase.png" />
        </v-col>
        <v-col>
          <img data-aos="fade-left" src="../assets/logos/windows.png" />
        </v-col>
      </v-row>
    </v-container>
  </div>
</template>

<script>
export default {};
</script>

<style lang="scss" scoped>
div {
  text-align: center;
}
img {
  height: 5rem;
}
.align {
  text-align: center;
}
</style>
