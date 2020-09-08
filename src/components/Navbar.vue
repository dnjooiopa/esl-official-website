<template>
  <div>
    <div id="navbar">
        <a>Home</a>
        <a>Activities & Awards</a>
        <a>Members</a>
        <a>Contact</a>
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
  justify-content: space-evenly;
}

</style>
