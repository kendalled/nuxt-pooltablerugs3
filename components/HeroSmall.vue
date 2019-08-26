<template>
  <section id="hero" class="hero is-dark is-halfheight has-text-centered">
    <div class="hero-body">
      <div class="container">
        <SizeSelect />
        <br>
        <p class="subtitle is-size-4">
          We'll find the perfect rug, just for you.
        </p>
      </div>
    </div>
  </section>
</template>

<script>
import SizeSelect from '~/components/SizeSelect'
export default {
  name: 'HeroSmall',
  components: {
    SizeSelect
  }
}
</script>

<style scoped>
#hero {
  background-image: linear-gradient(rgba(0, 0, 0, 0.7), rgba(0, 0, 0, 0.5 )), url('../assets/samplerug.jpg');
  background-size: cover;
  background-attachment: fixed;
}
</style>
