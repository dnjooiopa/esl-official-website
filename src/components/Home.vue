<template>
  <div>
    <img
      class="absolute h-sm-custom w-full object-cover object-center lg:h-64"
      src="../assets/images/home-img.jpg"
    />
  </div>
</template>

<script>
export default {
  name: "Home",
};
</script>

<style scoped>
.h-sm-custom {
  height: 30rem;
}

@media (min-width: 1024px) {
  .h-sm-custom {
    height: 44rem;
  }
}
</style>