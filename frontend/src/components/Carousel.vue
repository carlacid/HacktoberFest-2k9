<template>
    <div id="carousel">
      <b-carousel
      id="carousel-fade"
      style="text-shadow: 0px 0px 2px #000"
      fade
      indicators
      img-width="1024"
      img-height="300">
        <b-carousel-slide
        caption="First slide"
        img-src="https://picsum.photos/1024/480/?image=10"></b-carousel-slide>
        <b-carousel-slide
        caption="Second Slide"
        img-src="https://picsum.photos/1024/480/?image=12"></b-carousel-slide>
        <b-carousel-slide
        caption="Third Slide"
        img-src="https://picsum.photos/1024/480/?image=22"></b-carousel-slide>
      </b-carousel>
    </div>
</template>

<script>
export default {
    name: 'carousel'
}

var app = new Vue({
    name: 'carousel',
})
</script>

<style>

</style>