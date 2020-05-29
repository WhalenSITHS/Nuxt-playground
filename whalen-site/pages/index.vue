<template>
  <div>
    <v-app>
      <Splash />
      <About />
    </v-app>
  </div>
</template>

<script>
import Splash from "@/components/Splash";
import About from "@/components/About";

export default {
  components: {
    Splash,
    About
  }
};
</script>

<style lang="scss" scoped>
div {
  width: 100%;
}
.home {
  width: 100%;
  margin: 0 auto;
  text-align: center;
  display: flex;
  justify-content: center;
  align-items: center;
  flex-direction: column;
}
h1 {
}
</style>
