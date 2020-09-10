<template>
  <div class="activity-container">
    <div class="activity-title" v-on:click="onClick">Activity & Awards</div>
    
  </div>
</template>

<script>
export default {
  name: 'Activity',
}
</script>

<style>
.activity-container {
  display: flex;
  justify-content: center;
  margin-top: 108px;
}

.activity-title {
  font-size: 2.4rem;
  font-weight: 700;
  font-family: 'Orbitron', sans-serif;
}
</style>

<!-- 
<template>
    <b-carousel>
        <b-carousel-item v-for="(carousel, i) in carousels" :key="i">
            <section :class="`hero is-medium is-${carousel.color}`">
                <div class="hero-body has-text-centered">
                    <h1 class="title">{{carousel.text}}</h1>
                </div>
            </section>
        </b-carousel-item>
    </b-carousel>
</template>

<script>
export default {
    data(){
        return {
            carousels: [
                { text: 'Slide 1', color: 'primary' },
                { text: 'Slide 2', color: 'info' },
                { text: 'Slide 3', color: 'success' },
                { text: 'Slide 4', color: 'warning' },
                { text: 'Slide 5', color: 'danger' }
            ]
        }
    }
}
</script>
 -->