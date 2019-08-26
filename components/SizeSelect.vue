<template>
  <section class="has-text-centered">
    <h2 class="title">
      What size is your pool table?
    </h2>

    <b-field>
      <b-radio-button
        v-model="radioButton"
        native-value="8"
        :focusable="false"
      >
        8 Foot
      </b-radio-button>

      <b-radio-button
        v-model="radioButton"
        native-value="9"
      >
        9 Foot
      </b-radio-button>
      <b-radio-button
        v-model="radioButton"
        native-value="10"
      >
        10 Foot
      </b-radio-button>

      <b-radio-button
        v-model="radioButton"
        native-value="11"
      >
        11 Foot
      </b-radio-button>
    </b-field>
    <!-- <p class="content">
      <b>Selection:</b>
      {{ radioButton }}
    </p> -->
  </section>
</template>

<script>
export default {
  data () {
    return {
      radioButton: ''
    }
  }
}
</script>
