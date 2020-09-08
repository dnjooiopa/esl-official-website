<template>
  <div>
    <div class="navbar">
      <Navbar />
    </div>
    <div class="home">
      <Home />
    </div>
  </div>
</template>

<script>
//import EmployeeTable from './components/EmployeeTable'
import Home from './components/Home'
import Navbar from './components/Navbar'

export default {
  name: 'App',
  components: {
    Home,
    Navbar,
  },
}
</script>

<style></style>
