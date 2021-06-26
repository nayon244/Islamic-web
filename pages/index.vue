<template>
  <v-row>
    <v-col
      cols="12"
      xl="4"
      lg="4"
      md="12"
      sl="12"
      xs="12"
      v-for="(item, i) in doaData"
      :key="i"
    >
      <Card :data="item" />
    </v-col>
  </v-row>
</template>

<script>
export default {
  data: () => ({
    doaData: [
      {
        title: "Doa 1",
        content:
          "Doa kotha ekhane ase .... Doa kotha ekhane ase .... Doa kotha ekhane ase .... "
      },
      {
        title: "Doa 2",
        content:
          "Doa kotha ekhane ase .... Doa kotha ekhane ase .... Doa kotha ekhane ase .... "
      },
      {
        title: "Doa 3",
        content:
          "Doa kotha ekhane ase .... Doa kotha ekhane ase .... Doa kotha ekhane ase .... "
      },
      {
        title: "Doa 4",
        content:
          "Doa kotha ekhane ase .... Doa kotha ekhane ase .... Doa kotha ekhane ase .... "
      },
      {
        title: "Doa 5",
        content:
          "Doa kotha ekhane ase .... Doa kotha ekhane ase .... Doa kotha ekhane ase .... "
      },
      {
        title: "Doa 6",
        content:
          "Doa kotha ekhane ase .... Doa kotha ekhane ase .... Doa kotha ekhane ase .... "
      },
      {
        title: "Doa 7",
        content:
          "Doa kotha ekhane ase .... Doa kotha ekhane ase .... Doa kotha ekhane ase .... "
      }
    ]
  })
};
</script>
