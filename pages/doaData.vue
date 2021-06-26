<template>
  <pre>{{ doaDataItem }}</pre>
</template>
<script>
export default {
  data() {
    return {
      doaDataItem: {}
    };
  },
  mounted() {
    this.doaDataItem = this.$route.params;
    if (this.lodash.isEmpty(this.doaDataItem)) this.$router.push("/");
  }
};
</script>

<style lang="scss" scoped></style>
