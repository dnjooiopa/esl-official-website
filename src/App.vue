<template>
  <div>
    <Navbar />
    <Home />
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
    Navbar
  },
}
</script>

<style></style>
