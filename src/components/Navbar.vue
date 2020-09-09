<template>
  <div>
    <div id="navbar">
      <div id="nav-container">
        <div class="nav-item">
          <a>Home</a>
        </div>
        <div class="nav-item">
          <a>Activities & Awards</a>
        </div>
        <div class="nav-item">
          <a>Members</a>
        </div>
        <div class="nav-item">
          <a>Contact</a>
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
  width: 45%;
  height: 80px;
  display: flex;
  justify-content: space-between;
  align-items: center;

  font-size: 1.5rem;
  font-weight: 500;
  color: white;
  font-family: 'Orbitron', sans-serif;
}

.nav-item{
  height: 35px;
  padding:  10px;
}

.nav-item:hover {
  background-color: #E48305;
}
</style>
