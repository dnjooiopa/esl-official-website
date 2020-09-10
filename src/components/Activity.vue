<template>
  <div class="activity-container">
    <div class="activity-title">Activity & Awards</div>
    <br />
    <div class="slider-container">
      <b-carousel
        :pause-hover="pauseHover"
        :interval="interval"
        :indicator="indicator"
        :autoplay="autoplay"
        :icon-size="iconSize"
      >
        <b-carousel-item class="slider-item" v-for="(carousel, i) in carousels" :key="i">
          <div>
            <div class="title">{{carousel.text}}</div>
          </div>
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
      interval: 5000,
      indicator: false,
      autoplay: false,
      iconSize: "is-large",
      carousels: [
        { text: "Slide 1" },
        { text: "Slide 2" },
        { text: "Slide 3" },
        { text: "Slide 4" },
        { text: "Slide 5" },
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
  text-align: center;
  font-size: 2.4rem;
  font-weight: 700;
  font-family: "Orbitron", sans-serif;
}

.slider-container {
  width: 800px;
  margin-bottom: 300px;
}

.slider-item {
  display: flex;
  justify-content: flex-start;
  height: 400px;
}

.title {
  margin-top: 150px;
  text-align: center;
  font-size: 1.4rem;
  font-weight: 500;
  font-family: "Orbitron", sans-serif;
}
</style>