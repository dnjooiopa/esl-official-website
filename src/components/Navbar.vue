<template>
  <div>
    <div id="navbar">
      <div id="nav-container">
        <div class="nav-item">
          Home
        </div>
        <div class="nav-item">
          Activities & Awards
        </div>
        <div class="nav-item">
          Members
        </div>
        <div class="nav-item">
          Contact
        </div>
      </div>
    </div>
  </div>
</template>

<script>
export default {
  name: 'Navbar',
}
</script>

<style scoped>
#navbar {
  width: 100%;
  position: fixed;
  display: flex;
  justify-content: center;
}

#nav-container {
  width: 36%;
  height: 80px;
  display: flex;
  justify-content: space-between;
  align-items: center;

  font-size: 1.1rem;
  font-weight: 500;
  color: white;
  font-family: 'Orbitron', sans-serif;
}

.nav-item {
  height: 35px;
  padding: 10px;
}

.nav-item:hover {
  color: #e9ec16;
  cursor: pointer;
}
</style>
