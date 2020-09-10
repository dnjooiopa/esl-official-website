<template>
  <div>
    <div class="navbar" :class="{'navbar-toggle' :isToggle}">
      <div class="nav-container">
        <div class="nav-item">Home</div>
        <div class="nav-item">Activities & Awards</div>
        <div class="nav-item">Members</div>
        <div class="nav-item">Contact</div>
      </div>
    </div>
  </div>
</template>

<script>
export default {
  name: "Navbar",
  mounted() {
    window.onscroll = () => {
      if (window.scrollY > 680) {
        this.isToggle = true;
      } else {
        this.isToggle = false;
      }
    };
  },
  data() {
    return {
      isToggle: false,
    };
  },
};
</script>

<style scoped>
.navbar {
  width: 100%;
  position: absolute;
  display: flex;
  justify-content: center;
  background: transparent;
}

.nav-container {
  width: 36%;
  height: 72px;
  display: flex;
  justify-content: space-between;
  align-items: center;

  font-size: 1.1rem;
  font-weight: 500;
  color: white;
  font-family: "Orbitron", sans-serif;
}

.nav-item {
  height: 35px;
  padding: 10px;
}

.nav-item:hover {
  color: #e9ec16;
  cursor: pointer;
}

.navbar-toggle {
  position: fixed;
  background: #858a90;
}
</style>
