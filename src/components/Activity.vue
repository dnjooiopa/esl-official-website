<template>
  <div class="activity-container">
    <div class="activity-title">Activity & Awards</div>
    <div class="slider-container">
      <b-carousel
        :pause-hover="pauseHover"
        :autoplay="autoplay"
        :icon-size="iconSize"
        :indicator-style="indicatorStyle"
      >
        <b-carousel-item class="slider-item" v-for="(carousel, i) in carousels" :key="i">
          <div>
            <div class="description-container">
              <div class="description">{{carousel.text}}</div>
            </div>
            <div class="img-container">

            </div>
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
      autoplay: false,
      iconSize: "is-medium",
      indicatorStyle: "is-lines",
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
  margin-top: 140px;
}

.activity-title {
  text-align: center;
  font-size: 2.4rem;
  font-weight: 700;
  font-family: "Orbitron", sans-serif;
}

.slider-container {
  width: 1080px;
  margin: 24px 0px 300px;
}

.slider-item {
  display: flex;
  justify-content: flex-start;
  height: 540px;
  background-color: #2dd3a1;
}

.description-container {
  width: 240px;
  height: 100%;
  text-align: center;
}

.description {
  margin-top: 150px;
  font-size: 1.4rem;
  font-weight: 500;
  font-family: "Orbitron", sans-serif;
  color: black;
}
</style>