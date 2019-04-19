<template>
  <div id="app">
    <div class="container">
      <Header/>
    </div>
    <div class="container">
      <div class="columns">
        <Sidebar class="column is-3"/>
        <div class="column is-9">
          <div class="content">
            <Search/>
          </div>
          <div class="columns is-multiline is-mobile">
            <div class="column is-one-quarter-desktop is-half-mobile">
              <Store
                name="Vegan Mart"
                description="Our store offers a great supply of vegan and organic food"
                location="33540 Smallville, US"
                v-bind:isOnline="true"
              />
            </div>
            <div class="column is-one-quarter-desktop is-half-mobile">
              <Store
                name="Art Store"
                description="Our store offers a great supply of art"
                location="22145 Smallville, US"
                v-bind:isOnline="false"
              />
            </div>
            <div class="column is-one-quarter-desktop is-half-mobile">
              <Store
                name="Comics Mart"
                description="Our store offers a great supply of comics"
                location="99863 Smallville, US"
                v-bind:isOnline="true"
              />
            </div>
            <div class="column is-one-quarter-desktop is-half-mobile">
              <Store
                name="One Dollar Store"
                description="Buy anything for $1"
                location="33641 Smallville, US"
                v-bind:isOnline="false"
              />
            </div>
            <div class="column is-one-quarter-desktop is-half-mobile">
              <Store
                name="Vegan Mart"
                description="Our store offers a great supply of vegan and organic food"
                location="33540 Smallville, US"
                v-bind:isOnline="true"
              />
            </div>
            <div class="column is-one-quarter-desktop is-half-mobile">
              <Store
                name="Art Store"
                description="Our store offers a great supply of art"
                location="22145 Smallville, US"
                v-bind:isOnline="false"
              />
            </div>
            <div class="column is-one-quarter-desktop is-half-mobile">
              <Store
                name="Comics Mart"
                description="Our store offers a great supply of comics"
                location="99863 Smallville, US"
                v-bind:isOnline="true"
              />
            </div>
            <div class="column is-one-quarter-desktop is-half-mobile">
              <Store
                name="One Dollar Store"
                description="Buy anything for $1"
                location="33641 Smallville, US"
                v-bind:isOnline="false"
              />
            </div>
          </div>
        </div>
      </div>
    </div>
  </div>
</template>

<script>
import Header from "./components/Header.vue";
import Sidebar from "./components/Sidebar.vue";
import Search from "./components/Search.vue";
import Store from "./components/Store.vue";

export default {
  name: "app",
  components: {
    Header,
    Sidebar,
    Search,
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

body {
  margin-top: 12.5px;
  margin-bottom: 12.5px;
  margin-right: 20px;
  margin-left: 20px;
}
</style>
