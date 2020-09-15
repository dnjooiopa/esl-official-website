<template>
  <div class="flex h-sm-custom lg:h-64">
    <img class="w-full object-cover object-center" src="../assets/images/home-img.jpg" />
    <div class="absolute w-full mt-32 text-white text-center md:mt-48 lg:mt-64">
      <span class="text-4xl lg:text-5xl">
        Embedded
        <br class="md:hidden" />System
        <br class="md:hidden" />Laboratory
      </span>
    </div>
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