<template>
  <div>
    <div id="navbar">
      <div id="nav-container">
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
      console.log(window.scrollY);
      if (window.scrollY > 760) {
        document.getElementById("navbar").style.position = "fixed"
        document.getElementsByClassName("nav-item")[0].style.color = "black"
        document.getElementsByClassName("nav-item")[1].style.color = "black"
        document.getElementsByClassName("nav-item")[2].style.color = "black"
        document.getElementsByClassName("nav-item")[3].style.color = "black"
      }else{
        document.getElementById("navbar").style.position = "absolute"
        document.getElementsByClassName("nav-item")[0].style.color = "white"
        document.getElementsByClassName("nav-item")[1].style.color = "white"
        document.getElementsByClassName("nav-item")[2].style.color = "white"
        document.getElementsByClassName("nav-item")[3].style.color = "white"
      }
    };
  },
};
</script>

<style scoped>
#navbar {
  width: 100%;
  position: absolute;
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
</style>
