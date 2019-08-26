<template>
  <section id="hero" class="hero is-dark is-fullheight-with-navbar">
    <div class="hero-body">
      <div class="container">
        <h1 class="title">
          Protect your pool tables with style.
        </h1>
        <h2 class="subtitle">
          Custom sizing, shapes, and hundreds of designs.
        </h2>
        <b-button
          tag="nuxt-link"
          to="rugs"
          type="is-primary is-medium"
        >
          Shop Rugs
        </b-button>

        <b-button
          tag="nuxt-link"
          to="about"
          type="is-primary is-medium"
          inverted
        >
          Learn More
        </b-button>
      </div>
    </div>
  </section>
</template>

<script>
export default {
  name: 'Hero'
}

</script>

<style scoped>
#hero {
  background-image: linear-gradient(rgba(0, 0, 0, 0.3), rgba(0, 0, 0, 0.4)), url('https://pooltablerugs.firebaseapp.com/images/background.jpg');
  background-size: cover;
  background-attachment: fixed;
}
</style>
