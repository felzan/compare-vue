<template>
  <div id="app">
    <div class="navbar has-shadow">
      <div class="container">

        <div class="navbar-brand">
          <a class="navbar-item">felzan</a>
        </div>

        <span class="navbar-burger" v-on:click="toggleNavbar" v-bind:class="{'is-active': isActive}">
          <span></span>
          <span></span>
          <span></span>
        </span>

        <div class="navbar-menu" v-bind:class="{'is-active': isActive}">
          <div class="navbar-end">
            <router-link to="/" class="navbar-item r-item">Home</router-link>
            <router-link to="/faq" class="navbar-item r-item">Faq</router-link>
            <router-link to="/faq" class="navbar-item r-item">Home</router-link>
            <router-link to="/faq" class="navbar-item r-item">Home</router-link>
          </div>

          <div class="navbar-item">
            <p class="control">
              <a href="" class="button is-primary is-outlined">
                <span class="icon">
                  <i class="fa fa-download"></i>
                </span>
                <span>
                  Join now
                </span>
              </a>
            </p>
          </div>
        </div>

      </div>
    </div>

    <router-view/>

    <footer class="footer is-primary">
      <div class="container">
        <div class="columns">
          <div class="column">
            <p>Similique voluptas pariatur velit perferendis.</p>
          </div>
          <div class="column has-text-right">
            <a href="#" class="icon"><i class="fa fa-facebook"></i></a>
            <a href="#" class="icon"><i class="fa fa-twitter"></i></a>
          </div>
        </div>
      </div>
    </footer>

  </div>
</template>

<script>
export default {
  name: 'app',
  data: function() {
    return {
      isActive: false
    }
  },
  methods: {
    toggleNavbar: function() {
      this.isActive = !this.isActive
    }
  }
}
</script>

<style lang="sass">
@import '../node_modules/bulma/bulma.sass'
@import 'mq.sass'

.navbar
  background-color: #383838
  a:hover
    color: gray

.navbar-brand a
  color: #fff
  font-weight: bold

a.r-item
  color: #c1c1c1
  padding: 0.5rem 1.75rem
  +mobile
    color: gray
    &:hover
      background-color: #f1f1f1

// .navbar-menu span
//   background-color: #c1c1c1

footer
  background-color: $primary !important
  color: #fff

  .icon
    color: #fff
    margin-left: 20px
</style>
