<template>
  <div>
    <HeroSmall />
    <section class="container section">
      <div class="columns is-mobile">
        <card
          title="Free"
          icon="github-circle"
        />

        <card
          title="Responsive"
          icon="cellphone-link"
        />

        <card
          title="Modern"
          icon="alert-decagram"
        />
      </div>
      <div class="columns is-mobile">
        <card
          title="Free"
          icon="github-circle"
        />

        <card
          title="Responsive"
          icon="cellphone-link"
        />

        <card
          title="Modern"
          icon="alert-decagram"
        />
      </div>
    </section>
  </div>
</template>

<script>
import Card from '~/components/Card'
import HeroSmall from '~/components/HeroSmall'

export default {
  components: {
    Card,
    HeroSmall
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
