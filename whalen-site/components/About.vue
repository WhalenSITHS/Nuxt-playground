<template>
  <div>
    <v-container class="container">
      <h1 align-self="center" data-aos="fade-up">What We Do</h1>
      <v-row
        data-aos="flip-up"
        class="row light-blue darken-4"
        align-content="center"
      >
        <v-col class="col" cols="12" md="4">
          <h2>Front-End Development</h2>

          <p>
            Students learn industry standard HTML, SCSS and JavaScript skills
          </p>
          <v-btn class="btn" color="primary">Learn More</v-btn>
        </v-col>
        <v-col cols="12" md="4" class="col">
          <h2>Back-End Development</h2>

          <p>
            Students work with MongoDB, NodeJS and Firebase to learn
            authentication and REST API's
          </p>
          <v-btn class="btn" color="primary">Learn More</v-btn>
        </v-col>
        <v-col cols="12" md="4" class="col">
          <h2>Work-Based Learning</h2>

          <p>
            Students maintain the school IT Infrastructure through in-house
            internship oppurtunities
          </p>
          <v-btn class="btn" color="primary">Learn More</v-btn>
        </v-col>
      </v-row>
      <v-lazy>
        <LogoGallery></LogoGallery>
      </v-lazy>
    </v-container>
  </div>
</template>

<script>
import LogoGallery from "./LogoGallery";
export default {
  name: "About",
  components: {
    LogoGallery
  }
};
</script>

<style lang="scss" scoped>
.btn {
  margin: 0 1rem;
  transition: all 0.3s;
  color: white;
  align-self: center;
}
.btn:hover {
  background-color: #42a5f6;
  color: white;
}
.container {
  height: 95vh;
  margin: 2rem auto;
  color: black;
  background-color: #fff;
  text-align: center;
}
.col {
  text-align: center;
  display: flex;
  flex-direction: column;
  justify-content: space-between;
  align-items: center;
}

h1 {
  font-size: 4rem;
  text-transform: uppercase;
  margin: 2rem auto;
  text-align: center;
  border-bottom: 3px solid #42a5f6;
  display: inline-block;
}
h2 {
  text-align: center;
  font-family: sub-header-font;
  font-size: 2.2rem;
  font-style: italic;
  border-bottom: 3px solid #00c2ff;
  display: inline-block;
  text-transform: uppercase;
  margin: 1rem 0;
  padding: 1rem 0;
  color: white;
}
p {
  color: #cfd8dc;
  text-align: center;
  font-size: 1.2rem;
}
.row {
  height: 50vh;
  margin: 3rem auto;
  text-align: center;
}
@media only screen and (max-width: 960px) {
  .col {
    margin: 0.5rem auto;
  }
  .container {
    height: auto;
  }
  .row {
    height: auto;
    text-align: center;
    padding: 2rem auto;
    font-family: "Arvo", serif;
  }
  h1 {
    font-size: 2.5rem;
    margin: 1rem auto;
  }
  h2 {
    font-size: 1.8rem;
    margin: 1rem auto;
  }
  p {
    font-size: 1rem;
    margin: 1rem auto;
  }
  .btn {
    margin: 5px auto;
  }
}
</style>
