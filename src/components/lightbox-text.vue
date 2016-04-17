<template>
  <div class="doms-lightbox lightbox-caption" :style="{ width: width + 'px', height: height + 'px' }">
    <p class="doms-lightbox caption-text">{{text}}</p>
  </div>
</template>

<script>
export default {
  props: {
    text: String,
    width: Number,
    height: Number
  }
}
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped>
.doms-lightbox .lightbox-caption .caption-text {
  color: blue;
  text-align: center;
  width: 100%;
}

</style>
