<template>
  <div class="home-container">
    <div class="brand">
      <h1>Embedded System Laboratory</h1>
    </div>
    <img src="../assets/home-img.jpg" class="responsive" />
  </div>
</template>

<script>
export default {
  name: 'Home',
}
</script>

<style scoped>
.home-container {
  display: flex;
  justify-content: center;
}

.brand {
  position: absolute;
  margin-top: 310px;

  font-size: 2.1rem;
  font-weight: 900;
  color: white;
  font-family: 'Orbitron', sans-serif;
}

.responsive {
  max-width: 100%;
  height: auto;
}
</style>
