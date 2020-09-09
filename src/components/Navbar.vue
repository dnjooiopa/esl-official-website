<template>
  <div>
    <div id="navbar">
      <div id="nav-container">
        <a>Home</a>
        <a>Activities & Awards</a>
        <a>Members</a>
        <a>Contact</a>
      </div>
    </div>
  </div>
</template>

<script>
export default {
  name: 'Navbar',
}
</script>

<style>
#navbar {
  width: 100%;
  position: fixed;
  display: flex;
  justify-content: center;
}

#nav-container {
  width: 40%;
  height: 50px;
  display: flex;
  justify-content: space-between;
  align-items: center;
  font-size: 1.6rem;
  color: white;
}
</style>
