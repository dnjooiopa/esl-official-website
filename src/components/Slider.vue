<template>
  <div class="flex flex-col items-center my-8">
    <div class="img-container bg-white rounded overflow-x-hidden flex snap-x">
      <div class="snap-start w-full h-full flex flex-shrink-0 relative" id="slide-1">
        <img
          src="../assets/images/topgun-2020.jpg"
          class="h-full w-full object-cover absolute inset-0 z-10"
        />
      </div>
      <div class="snap-start w-full h-full flex flex-shrink-0 relative" id="slide-2">
        <img
          src="../assets/images/silicon-craft.jpg"
          class="h-full w-full object-cover object-bottom absolute inset-0 z-10"
        />
      </div>
      <div class="snap-start w-full h-full flex flex-shrink-0 bg-red-600" id="slide-3">Slide 3</div>
      <div class="snap-start w-full h-full flex flex-shrink-0 bg-orange-600" id="slide-4">Slide 4</div>
      <div class="snap-start w-full h-full flex flex-shrink-0 bg-purple-600" id="slide-5">Slide 5</div>
      <div class="snap-start w-full h-full flex flex-shrink-0 bg-black relative" id="slide-6">
        <img
          src="https://images.unsplash.com/photo-1556740738-b6a63e27c4df?ixlib=rb-1.2.1&ixid=eyJhcHBfaWQiOjEyMDd9&auto=format&fit=crop&w=448&q=80"
          class="h-full w-full object-cover absolute inset-0 z-10 opacity-25"
        />
        <h1 class="z-20 text-center">Any kind of content here, images too!</h1>
      </div>
    </div>

    <div class="flex mt-8">
      <a
        class="w-8 mr-1 h-8 text-gray-700 rounded-full bg-white flex justify-center items-center"
        href="#slide-1"
      >1</a>
      <a
        class="w-8 mr-1 h-8 text-gray-700 rounded-full bg-white flex justify-center items-center"
        href="#slide-2"
      >2</a>
      <a
        class="w-8 mr-1 h-8 text-gray-700 rounded-full bg-white flex justify-center items-center"
        href="#slide-3"
      >3</a>
      <a
        class="w-8 mr-1 h-8 text-gray-700 rounded-full bg-white flex justify-center items-center"
        href="#slide-4"
      >4</a>
      <a
        class="w-8 h-8 text-gray-700 rounded-full bg-white flex justify-center items-center"
        href="#slide-5"
      >5</a>
      <a
        class="w-8 h-8 text-gray-700 rounded-full bg-white flex justify-center items-center"
        href="#slide-6"
      >6</a>
      <a
        class="w-8 h-8 text-gray-700 rounded-full bg-white flex justify-center items-center"
        :href="prev"
      >prev</a>
      <a
        class="w-8 h-8 text-gray-700 rounded-full bg-white flex justify-center items-center"
        :href="next"
      >next</a>
    </div>
  </div>
</template>

<script>
export default {
  name: "Slider",
  data() {
    return {
      prev: "#slide-1",
      next: "#slide-2",
    };
  },
};
</script>

<style>
.snap-x {
  scroll-snap-type: x mandatory;

  scroll-behavior: smooth;
  -webkit-overflow-scrolling: touch;
}

.snap-start {
  scroll-snap-align: start;
}

.img-container {
  width: 300px;
  height: 225px;
}

@media (min-width: 768px) {
  .img-container {
    width: 720px;
    height: 540px;
  }

  @media (min-width: 1200px) {
    .img-container {
      width: 840px;
      height: 540px;
    }
  }
}
</style>