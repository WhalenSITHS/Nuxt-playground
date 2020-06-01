<template>
  <v-app>
    <v-app-bar class="hidden-sm-and-down" app fixed color="#fff">
      <v-toolbar-title>
        <img class="logo" src="../static/v.png" />
      </v-toolbar-title>
      <v-spacer></v-spacer>

      <nuxt-link class="nuxt-link" to="/">
        <v-btn outlined class="btn" active-class="no-active">Home</v-btn>
      </nuxt-link>

      <nuxt-link class="nuxt-link" to="/studentwork">
        <v-btn outlined class="btn" active-class="no-active">Student Work</v-btn>
      </nuxt-link>
      <nuxt-link class="nuxt-link" to="/Resources">
        <v-btn outlined class="btn" active-class="no-active">Resources</v-btn>
      </nuxt-link>
      <v-btn outlined class="btn" active-class="no-active">What I'm Learning</v-btn>
      <v-btn outlined active-class="no-active" class="btn">Curriculum</v-btn>
    </v-app-bar>
    <v-app-bar class="hidden-md-and-up">
      <v-btn icon>
        <img
          src="../static/iconfinder_menu-alt_134216.svg"
          @click="drawer = !drawer"
          class="black--text icon"
        />
      </v-btn>
    </v-app-bar>
    <v-navigation-drawer app v-model="drawer" class="secondary my-nav" width="80%">
      <v-list>
        <v-list-item-group class="test" color="primary">
          <v-list-item class="white my-4">
            <nuxt-link class="route nuxt-link" to="/">Home</nuxt-link>
          </v-list-item>
          <v-list-item class="white my-4">
            <nuxt-link class="route nuxt-link" to="/studentwork">Student Work</nuxt-link>
          </v-list-item>
          <v-list-item class="white my-4">
            <nuxt-link class="route nuxt-link" to="/Resources">Resources</nuxt-link>
          </v-list-item>
          <v-list-item class="white my-4">
            <nuxt-link class="route nuxt-link" to="/home">What I'm Learning</nuxt-link>
          </v-list-item>
          <v-list-item class="white my-4">
            <nuxt-link class="route nuxt-link" to="/home">Curriculum</nuxt-link>
          </v-list-item>
        </v-list-item-group>
      </v-list>
    </v-navigation-drawer>
    <nuxt />
  </v-app>
</template>

<script>
export default {
  data() {
    return {
      drawer: false
    };
  }
};
</script>

<style lang="scss" scoped>
.icon {
  height: 2rem;
}
.logo {
  height: 2.2rem;
}

.v-btn--active.no-active::before {
  opacity: 0 !important;
}
.btn {
  margin: 0 1rem;
  transition: all 0.3s;
}

.btn:hover {
  background-color: #42a5f6;
  color: white;
}
.test {
  color: black;
}
.route {
  text-align: center;

  margin: 0 auto;
}
.my-nav {
  text-align: center;
}
</style>
