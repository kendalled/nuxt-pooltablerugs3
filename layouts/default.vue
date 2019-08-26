<template>
  <!-- THIS IS THE ROOT BODY TAG -->
  <div class="has-navbar-fixed-top">
    <b-navbar class="navbar" fixed-top>
      <template slot="brand">
        <b-navbar-item href="/">
          <img
            src="https://raw.githubusercontent.com/buefy/buefy/dev/static/img/buefy-logo.png"
            alt="Lightweight UI components for Vue.js based on Bulma"
          >
        </b-navbar-item>
      </template>
      <template slot="start">
        <nuxt-link
          v-for="(item, key) of items"
          :key="key"
          :to="item.to.name"
          class="navbar-item"
          exact-active-class="nuxt-link-exact-active"
          exact
        >
          {{ item.title }}
        </nuxt-link>
      </template>

      <template slot="end">
        <b-navbar-item tag="div">
          <div class="buttons">
            <b-button
              type="is-success"
              icon-right="cart"
            >
              Cart
            </b-button>
          </div>
        </b-navbar-item>
        <b-dropdown position="is-bottom-left" aria-role="menu">
          <a
            slot="trigger"
            class="navbar-item"
            role="button"
          >
            <span>Account</span>
            <b-icon icon="menu-down" />
          </a>

          <b-dropdown-item
            aria-role="menu-item"
            :focusable="false"
            custom
            paddingless
          >
            <form action="">
              <div class="modal-card" style="width:300px;">
                <section class="modal-card-body">
                  <b-field label="Email">
                    <b-input
                      type="email"
                      placeholder="Your email"
                      required
                    />
                  </b-field>

                  <b-field label="Password">
                    <b-input
                      type="password"
                      password-reveal
                      placeholder="Your password"
                      required
                    />
                  </b-field>

                  <b-checkbox>Remember me</b-checkbox>
                </section>
                <footer class="modal-card-foot">
                  <button class="button is-primary">
                    Login
                  </button>
                  <b-button
                    type="button is-primary"
                    outlined
                  >
                    <strong>Sign up</strong>
                  </b-button>
                </footer>
              </div>
            </form>
          </b-dropdown-item>
        </b-dropdown>
      </template>
    </b-navbar>
    <section class="main-content columns">
      <div id="pagewrapper" class="container column is-fluid">
        <nuxt />
      </div>
    </section>
    <footer class="footer is-dark">
      <div class="content has-text-centered">
        <p>
          &copy; 2019 The Pool Table Store | <strong>Pool Table Rugs</strong> by <a href="https://github.com/kendalled">KJ</a> |
          License: <a href="http://creativecommons.org/licenses/by-nc-sa/4.0/">MIT License</a>.
        </p>
      </div>
    </footer>
  </div>
</template>

<script>
export default {
  data () {
    return {
      components: {
      },
      items: [
        {
          title: 'Home',
          icon: 'home',
          to: { name: '/' }
        },
        {
          title: 'Rugs',
          icon: 'home',
          to: { name: 'rugs' }
        },
        {
          title: 'About Us',
          icon: 'lightbulb',
          to: { name: 'about' }
        }
      ]
    }
  }
}
</script>

<style scoped>
#pagewrapper {
  margin: 0 auto !important;
}
.nuxt-link-exact-active {
  color: #4a4a4a !important;
  background: #fff;
}
.page-fade-enter-active, .page-fade-leave-active {
  transition: opacity .3s ease;
}
.page-fade-enter, .page-fade-leave-to
/* .component-fade-leave-active below version 2.1.8 */ {
  opacity: 0;
}

/*
.is-active {
  background: #fff;
  color: #1f1f1f;
} */
</style>
