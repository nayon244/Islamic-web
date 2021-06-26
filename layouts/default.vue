<template>
  <v-app dark>
    <v-app-bar app flat color="blue">
      <v-spacer></v-spacer>
      <span class="white--text">
        <v-btn
          @click="goToHome"
          dark
          depressed
          x-large
          color="blue lighten-1"
          rounded
        >
          <b> {{ title }} </b>
        </v-btn>
      </span>
      <v-spacer></v-spacer>
    </v-app-bar>
    <v-main>
      <v-container>
        <nuxt />
      </v-container>
    </v-main>
  </v-app>
</template>

<script>
export default {
  data() {
    return {
      clipped: false,
      drawer: false,
      fixed: false,
      items: [
        {
          icon: "mdi-apps",
          title: "Welcome",
          to: "/"
        },
        {
          icon: "mdi-chart-bubble",
          title: "Inspire",
          to: "/inspire"
        }
      ],
      miniVariant: false,
      right: true,
      rightDrawer: false,
      title: "আয়তুল কুরসী"
    };
  },
  methods: {
    goToHome() {
      this.$router.push("/");
    }
  }
};
</script>
