<template>
  <div>
    <Hero />
    <section class="section">
      <br>
      <br>
      <h2 class="title">
        Subheading Goes Here
      </h2>

      <h3 class="subtitle">
        And Content for the Homepage.
      </h3>

      <br>
      <p>
        Lorem, ipsum dolor sit amet consectetur adipisicing elit. Earum dolor inventore corporis nostrum officiis nemo numquam ipsum? Vitae ab dolore aspernatur, velit repellendus sequi recusandae quae aliquid nulla incidunt? Aperiam?
      </p>
      <br>
      <p>
        Lorem, ipsum dolor sit amet consectetur adipisicing elit. Earum dolor inventore corporis nostrum officiis nemo numquam ipsum? Vitae ab dolore aspernatur, velit repellendus sequi recusandae quae aliquid nulla incidunt? Aperiam?
      </p>
      <br>
      <p>
        Lorem, ipsum dolor sit amet consectetur adipisicing elit. Earum dolor inventore corporis nostrum officiis nemo numquam ipsum? Vitae ab dolore aspernatur, velit repellendus sequi recusandae quae aliquid nulla incidunt? Aperiam?
      </p>
    </section>
  </div>
</template>

<script>
import Hero from '~/components/Hero'

export default {
  name: 'HomePage',
  components: {
    Hero
  },
  transition: {
    name: 'page-fade',
    mode: 'out-in',
    enterActiveClass: 'page-fade-enter-active',
    leaveActiveClass: 'page-fade-leave-active',
    enterClass: 'page-fade-enter',
    leaveToClass: 'page-fade-leave-to'
  }
}
</script>

<style scoped>
</style>
