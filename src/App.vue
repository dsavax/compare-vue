<template>
  <div id="app">
    <nav class="navbar" role="navigation" aria-label="main navigation">
      <div class="container">
        <div class="navbar-brand">
          <a class="navbar-item">My Company</a>

          <a role="button" class="navbar-burger" aria-label="menu" aria-expanded="false">
            <span aria-hidden="true"></span>
            <span aria-hidden="true"></span>
            <span aria-hidden="true"></span>
          </a>

          <div class="navbar-menu">
              <div class="navbar-end">
                <router-link to="/" class="navbar-item navbar-end">Home</router-link>
                <router-link to="faq" class="navbar-item navbar-end">Features</router-link>
                <router-link to="faq" class="navbar-item navbar-end">About</router-link>
                <router-link to="faq" class="navbar-item navbar-end">FAQ</router-link>

                <div class="navbar-item">
                  <p class="control">
                    <a class="button is-primary is-outlined">
                      <span class="icon">
                        <i class="fa fa-download"></i>
                      </span>
                      <span>Join Now</span>
                    </a>
                  </p>
                </div>
              </div>
          </div>
        </div>
      </div>
    </nav>
    <router-view></router-view>
  </div>
</template>

<script>
export default {
  name: 'App'
}
</script>

<style lang="sass">
@import '../node_modules/bulma/bulma.sass'
@import 'mq'

.navbar
  background-color: #383838
  a:hover
  color: gray

.navbar-brand a
  color: #fff
  font-weight: bold

.navbar-end a
  font-weight: normal

.navbar-end a
  color:#C1C1C1
  padding: 0.5rem 1.75rem
  +mobile
    color: gray
    &:hover
      background-color: #F1F1F1



</style>
