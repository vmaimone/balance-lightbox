<template>
  <div id="app">
    <h1>Demo</h1>
    <lightbox-page
      :options=" {
        src: 'http://i0.wp.com/balancewebster.com/home/wp-content/uploads/2016/04/mb3.jpg?zoom=2&amp;resize=780%2C585',
        caption: 'Lorem ipsum dolor sit amet, consectetur adipisicing elit. Voluptatibus, a? Ipsum, aliquid! Commodi natus aperiam cum adipisci voluptates illum nihil explicabo minus fuga odio qui, vitae temporibus laboriosam ducimus ut.',
        width: 780,
        height: 585
      } ">
   </lightbox-page>
  </div>
</template>

<script>
import lightboxPage from './components/lightbox-page.vue'

export default {
  components: {
    lightboxPage
  }
}
</script>

<style>
html {
  height: 100%;
}

body {
  display: flex;
  align-items: center;
  justify-content: center;
  height: 100%;
}

#app {
  color: #2c3e50;
  margin-top: -100px;
  max-width: 600px;
  font-family: Source Sans Pro, Helvetica, sans-serif;
  text-align: center;
}

#app a {
  color: #42b983;
  text-decoration: none;
}
</style>
