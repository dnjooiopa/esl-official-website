<template>
  <div id="app">
    <Home />
    <Activity />
  </div>
</template>

<script>
import Home from "./components/Home";
import Activity from "./components/Activity";

export default {
  name: "App",
  components: { Home, Activity },
};
</script>

<style>
</style>
