<template>
  <a class="button has-background-success" href="#">{{ state }}</a>
</template>

<script>
export default {
  name: "HelloWorld",
  props: {
    state: Boolean,
  },
};
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped lang="sass">

a
  width: 70px
  height: 70px
</style>
