<template>
  <div class="activity-container">
    <div class="activity-title" v-on:click="onClick">Activity & Awards</div>
    
  </div>
</template>

<script>
export default {
  name: 'Activity',
  methods:{
      onClick(){
          alert("on click")
      }
  },
  mounted() {
  }
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
