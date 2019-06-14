<template>
  <div>
    <navbar/>
    <section class="hero is-dark is-small header-image">
      <!-- Hero head: will stick at the top -->
      <div class="hero-head"></div>

      <!-- Hero content: will be in the middle -->
      <div class="hero-body">
        <div class="container columns level">
          <div class="column has-text-centered is-half level-left">
            <h1 class="title is-2">The ultimate CS skills</h1>
            <h3 class="is-size-4">challenge in Africa.</h3>
            <br>
            <div class="space">
              <nuxt-link class="button is-danger is-outlined is-medium" to="insights">Learn more</nuxt-link>
            </div>
          </div>
          <div class="column is-half level-right">
            <img width="100%" height="50%" src="~/assets/img/coder.svg" class="step__image">
          </div>
        </div>
      </div>
    </section>
    <br>
    <br>
    <feature/>
    <br>
    <br>
    <partners/>
  </div>
</template>

<script>
import Navbar from "~/components/Navbar";
import Feature from "~/components/Feature";
import Partners from "~/components/Partners";

export default {
  components: {
    Navbar,
    Feature,
    Partners
  }
};
</script>

<style>
</style>
