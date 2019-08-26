<template>
  <div class="column">
    <div class="card">
      <header class="card-header">
        <p class="card-header-title has-text-grey">
          {{ title }}
        </p>
      </header>
      <div class="card-image">
        <figure class="image is-4by3">
          <img src="../assets/rug1.png" alt="Placeholder image">
        </figure>
      </div>
      <!-- <div class="content has-text-centered">
        </div> -->
      <footer class="card-footer">
        <div class="card-footer-item">
          <span>
            <div class="buttons">
              <b-button rounded type="is-small">
                Details
              </b-button>
              <b-button rounded type="is-primary is-small">
                Add to Cart
              </b-button>
            </div>
          </span>
        </div>
      </footer>
    </div>
  </div>
</template>

<script>
export default {
  props: {
    title: {
      type: String,
      required: true
    },
    icon: {
      type: String,
      required: true
    }
  }
}
</script>

<style scoped>
.card {
  border-radius: 4px;
}
</style>
