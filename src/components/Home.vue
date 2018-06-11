<template>
  <div class="home">
      <section class="hero">
        <div class="hero-body">
          <div class="container">
            <h1 class="title">{{ heading }}</h1>
            <div class="is-two-thirds column is-paddingless">
              <h2 class="subtitle is-4">{{ subheading}}</h2>
            </div>
            <a class="button is-large is-primary" id="learn">Learn more</a>
          </div>
        </div>
      </section>
  </div>
</template>

<script>
export default {
  name: 'Home',
  data () {
    return {
      heading: 'Soaring to new heights',
      subheading: 'Lorem isum dolor sit amet, и немного рыбы на русском жфывдлаофжывлдрпшгукрщшпг.'
    }
  }
}
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style lang="sass" scoped>
@import '../mq'

.hero
 background: url('../assets/clouds.jpg')
 background-size: cover

 .title
  +mobile
    font-weight: bold
  +tablet
    font-size: 2.5rem
  +desktop
    font-size: 4rem
    margin-top: 2rem

  h2
    margin: 1.5rem 0 2rem 0 !important

</style>
