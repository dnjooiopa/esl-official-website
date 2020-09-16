<template>
  <div id="app">
    <Home />
    <Activity />
    <Slider />
  </div>
</template>

<script>
import Home from "./components/Home";
import Activity from "./components/Activity";
import Slider from "./components/Slider"

export default {
  name: "App",
  components: { Home, Activity, Slider },
};
</script>

<style>
</style>
