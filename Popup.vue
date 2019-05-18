<template>
  <nav class="beevesagent is-overlay">
    <div class="card is-3">
      <header class="card-header">
        <p class="card-header-title">Component</p>
        <a href="#" class="card-header-icon" aria-label="more options">
          <span class="icon">
            <i class="fas fa-angle-down" aria-hidden="true"></i>
          </span>
        </a>
      </header>
      <div class="card-content">
        <div class="content">
          Lorem ipsum dolor sit amet, consectetur adipiscing elit. Phasellus nec iaculis mauris.
          <a
            href="#"
          >@bulmaio</a>.
          <a href="#">#css</a>
          <a href="#">#responsive</a>
          <br>
          <time datetime="2016-1-1">11:09 PM - 1 Jan 2016</time>
        </div>
      </div>
      <footer class="card-footer">
        <a href="#" class="card-footer-item">Save</a>
        <a href="#" class="card-footer-item">Edit</a>
        <a href="#" class="card-footer-item">Delete</a>
      </footer>
    </div>
  </nav>
</template>

<script>
import Vue from "vue";
import Buefy from "buefy";
Vue.use(Buefy);

export default {
  data() {
    return {
      message: "Hello, I'm a browser extension!"
    };
  }
};
</script>
 <style scoped lang="scss">
// Import Bulma's core

.beevesagent {
  @import "~bulma/sass/utilities/_all";
  z-index: 999;
  position: fixed;
  top: 2em;
  right: 2em;
  // Set your colors
  $primary: #8c67ef;
  $primary-invert: findColorInvert($primary);
  $twitter: #4099ff;
  $twitter-invert: findColorInvert($twitter);

  // Setup $colors to use as bulma classes (e.g. 'is-twitter')
  $colors: (
    "white": (
      $white,
      $black
    ),
    "black": (
      $black,
      $white
    ),
    "light": (
      $light,
      $light-invert
    ),
    "dark": (
      $dark,
      $dark-invert
    ),
    "primary": (
      $primary,
      $primary-invert
    ),
    "info": (
      $info,
      $info-invert
    ),
    "success": (
      $success,
      $success-invert
    ),
    "warning": (
      $warning,
      $warning-invert
    ),
    "danger": (
      $danger,
      $danger-invert
    ),
    "twitter": (
      $twitter,
      $twitter-invert
    )
  );

  // Links
  $link: $primary;
  $link-invert: $primary-invert;
  $link-focus-border: $primary;

  // Import Bulma and Buefy styles
  @import "~bulma";
  @import "~buefy/src/scss/buefy";
}
</style>



