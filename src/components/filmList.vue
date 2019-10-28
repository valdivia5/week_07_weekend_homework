<template lang="html">
</template>

<script>
export default {
  name: "studio-ghibli-films-list",
  props: ["films"],
  components: {

  }
};
</script>

<style lang="css" scoped>
.film-list {
  width: 45%;
  height: 550px;
  overflow-y: scroll;
  display: flex;
  flex-wrap: wrap;
}
</style>
