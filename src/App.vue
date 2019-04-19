<template>
  <div id="app">
    <city-header
      city="Smallville"
      fillColor="#fff"
      imgUrl="https://upload.wikimedia.org/wikipedia/commons/b/bd/Eulo_Bore.jpg"
    />
    <section class="section">
      <div class="container">
        <div class="columns">
          <sidebar class="column is-3"/>
          <div class="column is-9">
            <div class="content">
              <search/>
            </div>
            <div class="columns is-multiline is-mobile">
              <div class="column is-one-quarter-desktop is-one-third-tablet is-half-mobile">
                <store
                  name="Vegan Mart"
                  description="Our store offers a great supply of vegan and organic food"
                  location="33540 Smallville, US"
                  v-bind:isOnline="true"
                />
              </div>
              <div class="column is-one-quarter-desktop is-one-third-tablet is-half-mobile">
                <store
                  name="Art Store"
                  description="Our store offers a great supply of art"
                  location="22145 Smallville, US"
                  v-bind:isOnline="false"
                />
              </div>
              <div class="column is-one-quarter-desktop is-one-third-tablet is-half-mobile">
                <store
                  name="Comics Mart"
                  description="Our store offers a great supply of comics"
                  location="99863 Smallville, US"
                  v-bind:isOnline="true"
                />
              </div>
              <div class="column is-one-quarter-desktop is-one-third-tablet is-half-mobile">
                <store
                  name="One Dollar Store"
                  description="Buy anything for $1"
                  location="33641 Smallville, US"
                  v-bind:isOnline="false"
                />
              </div>
              <div class="column is-one-quarter-desktop is-one-third-tablet is-half-mobile">
                <store
                  name="Vegan Mart"
                  description="Our store offers a great supply of vegan and organic food"
                  location="33540 Smallville, US"
                  v-bind:isOnline="true"
                />
              </div>
              <div class="column is-one-quarter-desktop is-one-third-tablet is-half-mobile">
                <store
                  name="Art Store"
                  description="Our store offers a great supply of art"
                  location="22145 Smallville, US"
                  v-bind:isOnline="false"
                />
              </div>
              <div class="column is-one-quarter-desktop is-one-third-tablet is-half-mobile">
                <store
                  name="Comics Mart"
                  description="Our store offers a great supply of comics"
                  location="99863 Smallville, US"
                  v-bind:isOnline="true"
                />
              </div>
              <div class="column is-one-quarter-desktop is-one-third-tablet is-half-mobile">
                <store
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
    </section>
  </div>
</template>

<script>
import CityHeader from "./components/CityHeader.vue";
import Sidebar from "./components/Sidebar.vue";
import Search from "./components/Search.vue";
import Store from "./components/Store.vue";

export default {
  name: "app",
  components: {
    CityHeader,
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
</style>
