<template>
  <div class="activity-container">
    <div class="activity-title">Activity & Awards</div>
    <br />
    <div class="slider-container">
      <b-carousel :pause-hover="pauseHover" :interval="interval">
        <b-carousel-item v-for="(carousel, i) in carousels" :key="i">
          <section :class="`hero is-medium is-${carousel.color}`">
            <div class="hero-body has-text-centered">
              <h1 class="title">{{carousel.text}}</h1>
            </div>
          </section>
        </b-carousel-item>
      </b-carousel>
    </div>
  </div>
</template>

<script>
import Vue from "vue";
import Buefy from "buefy";
import "buefy/dist/buefy.css";

Vue.use(Buefy);

export default {
  name: "Activity",
  data() {
    return {
      pauseHover: false,
      interval: 3000,
      carousels: [
        { text: "Slide 1", color: "primary" },
        { text: "Slide 2", color: "info" },
        { text: "Slide 3", color: "success" },
        { text: "Slide 4", color: "warning" },
        { text: "Slide 5", color: "danger" },
      ],
    };
  },
};
</script>

<style scoped>
.activity-container {
  display: flex;
  flex-wrap: wrap;
  flex-direction: column;
  align-content: center;
  margin-top: 108px;
}

.activity-title {
  font-size: 2.4rem;
  font-weight: 700;
  font-family: "Orbitron", sans-serif;
}

.slider-container {
  width: 300px;
  margin-bottom: 300px;
}
</style>