<template>
  <div class="doms-lightbox lightbox-image" :style="{ width: width + 'px', height: height + 'px' }">
    <img
      slot="image"
      class="wp-image-2875"
      :src="imageSrc"
      :width="width"
      :height="height"
      scale="2"
    />
  </div>
</template>

<script>
export default {
  props: {
    imageSrc: String,
    width: Number,
    height: Number
  },
}
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped>
.doms-lightbox .lightbox-image {
  /* custom css here */
}
</style>
