<template>
  <img
    :src="url"
    alt="User profile image"
    class="h-10 w-10 rounded-3xl object-contain"
  />
</template>

<script>
export default {
  name: "ProfileImage",
  data() {
    return {
      url: "https://i.pravatar.cc/300",
    };
  },
};
</script>

<style lang="scss" scoped></style>
