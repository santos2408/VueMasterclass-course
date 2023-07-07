<template>
  <h1>Jobs Page {{ currentJobId }}</h1>
</template>

<script>
export default {
  name: "JobView",
  computed: {
    currentJobId() {
      console.log(this.$route);
      return this.$route.params.id;
    },
  },
};
</script>
