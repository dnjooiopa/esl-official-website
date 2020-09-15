<template>
  <div class="flex h-sm-custom lg:h-64">
    <img class="w-full object-cover object-center" src="../assets/images/home-img.jpg" />
    <div class="absolute brand text-white">Embedded System Laboratory</div>
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

.brand {
  left: 50%;
  transform: translate(-50%, -50%);
  top: 330px;
}

@media (min-width: 1024px) {
  .h-sm-custom {
    height: 44rem;
  }
}
</style>