<template>
  <div>
    <v-card flat color="white" @click="cardClicked">
      <v-toolbar>
        {{ data.title }}
        <v-spacer></v-spacer>
        <v-icon>mdi-chevron-right-circle-outline</v-icon>
      </v-toolbar>
    </v-card>
  </div>
</template>

<script>
export default {
  props: ["data"],
  methods: {
    cardClicked(event) {
      console.log(event);
      this.$router.push({ name: "inspire", params: this.data });
      //   this.$router.push("/inspire");
    }
  }
};
</script>

<style lang="sass" scoped></style>
