<template>
  <div class="container">
    <h1 class="statement">The amazing new Website is coming soon</h1>
    <p class="subtext">It's revolutionary due to it will change the world of <UserAgent /> websites as we know it</p>
    <p class="subtext">Be sure to sign-up to find out more about the next generation of websites
    and follow our progress</p>

    <!-- nuxt-link es para crear links entre las páginas de nuestra aplicación -->
    <nuxt-link to="/learnMore" class="callToAction">Learn More</nuxt-link>
    <nuxt-link to="/progress" class="callToAction">See Our Progress</nuxt-link>
    <nuxt-link to="/contact" class="callToAction">Contact Us</nuxt-link> 

  </div>
</template>

<script>
import UserAgent from '../components/UserAgent';

export default {
  components: {
    UserAgent
  }
}
</script>

<style>

</style>
