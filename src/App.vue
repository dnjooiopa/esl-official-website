<template>
  <div>
    <div>
      <Navbar />
    </div>
    <div>
      <Home />
    </div>
    <div>
      <Activity />
    </div>
  </div>
</template>

<script>
import Home from './components/Home'
import Navbar from './components/Navbar'
import Activity from './components/Activity'

export default {
  name: 'App',
  components: {
    Home,
    Navbar,
    Activity,
  },
}
</script>

<style></style>
