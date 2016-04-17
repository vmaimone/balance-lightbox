<template>
 <div class="doms-lightbox lightbox-page">
  <lightbox-image
    :image-src="options.src"
    :width="options.width"
    :height="options.height">
  </lightbox-image>
  <lightbox-text
    :text="options.caption"
    :width="options.width">
  </lightbox-text>
</div>
</template>

<script>
import lightboxImage from './lightbox-image.vue'
import lightboxText from './lightbox-text.vue'
export default {
  components: { lightboxText, lightboxImage },
  props: {
    options: {
      type: Object,
      default() {
        return {
          src: null,
          caption: ''
        }
      }
    }
  }
}
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped>
.doms-lightbox .lightbox-page {
  /* custom css here */
}
</style>
