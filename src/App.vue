<template>
  <div id="app">
    <div class="columns is-multiline">
      <div class="column">
        <Store
          name="Vegan Mart"
          description="Our store offers a great supply of vegan and organic food"
          location="33540 Smallville, US"
          v-bind:isOnline="true"
        />
      </div>
      <div class="column">
        <Store
          name="Art Store"
          description="Our store offers a great supply of art"
          location="22145 Smallville, US"
          v-bind:isOnline="false"
        />
      </div>
      <div class="column">
        <Store
          name="Comics Mart"
          description="Our store offers a great supply of comics"
          location="99863 Smallville, US"
          v-bind:isOnline="true"
        />
      </div>
      <div class="column">
        <Store
          name="One Dollar Store"
          description="Buy anything for $1"
          location="33641 Smallville, US"
          v-bind:isOnline="false"
        />
      </div>
    </div>
  </div>
</template>

<script>
import Store from "./components/Store.vue";

export default {
  name: "app",
  components: {
    Store
  }
};
</script>

<style lang="scss">
// Import Bulma's core
@import "~bulma/sass/utilities/_all";

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

.store {
  display: flex;
  flex-direction: column;
  height: 100%;
}
</style>
