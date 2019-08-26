<template>
  <div>
    <section class="section">
      <br>
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

        <card
          title="Lightweight"
          icon="arrange-bring-to-front"
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

        <card
          title="Lightweight"
          icon="arrange-bring-to-front"
        />
      </div>
    </section>
  </div>
</template>

<script>
import Card from '~/components/Card'
export default {
  components: {
    Card
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
