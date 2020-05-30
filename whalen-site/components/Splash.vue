<template>
  <v-container class="container">
    <div class="full">
      <div class="wrapper">
        <h1>Michael Whalen</h1>
        <h2>High School Computer Science and Web Engineering</h2>
      </div>
    </div>
  </v-container>
</template>

<script>
export default {};
</script>

<style lang="scss" scoped>
.full {
  background-image: linear-gradient(
      to right,
      rgba(66, 165, 246, 0.5),
      rgba(5, 11, 31, 0.5)
    ),
    url("../assets/geo.jpg");
  background-size: cover;
  height: 90vh;
  color: white;
  position: relative;
}
.column {
  padding: 3rem;
}

h1 {
  font-size: 3rem;

  text-transform: uppercase;
  margin: 1rem 0;
}
h2 {
  font-family: sub-header-font;
  font-size: 1.5rem;
  font-style: italic;
  margin: 1rem 0;
}

.wrapper {
  position: absolute;
  top: 50%;
  left: 50%;
  transform: translate(-50%, -50%);
}
.container {
  margin-top: 5rem;
}
@media only screen and (max-width: 960px) {
  .wrapper {
    width: 100%;
    text-align: center;
  }
  h1 {
    font-size: 2.5rem;
  }
  h2 {
    font-size: 1.2rem;
  }
  .container {
    height: auto;
    margin-top: 5px;
  }
}
</style>
