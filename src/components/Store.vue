<template>
  <div class="store card">
    <div class="card-image">
      <figure class="image is-4by3">
        <img src="https://bulma.io/images/placeholders/1280x960.png" alt="Placeholder image">
      </figure>
    </div>
    <div class="card-content">
      <div class="media">
        <div class="media-content">
          <div class="title is-size-5 is-size-4-mobile" style="margin-bottom: 2px;">{{name}}</div>
          <small v-if="isOnline">
            <b-icon icon="circle" size="is-small" type="is-success"></b-icon>
            <span class="is-size-7 is-size-6-mobile" style="margin-left:3px;">Online</span>
          </small>
          <small v-else>
            <b-icon icon="circle" size="is-small"></b-icon>
            <span class="is-size-7 is-size-6-mobile" style="margin-left:3px;color:gray;">Offline</span>
          </small>
        </div>
      </div>

      <div class="content">
        <p class="is-size-6-tablet">{{description}}</p>
      </div>
    </div>
    <div class="card-footer">
      <small>
        <b-icon icon="map-marker" size="is-small"/>
        <span class="is-size-7-tablet" style="margin-left:3px;">{{location}}</span>
      </small>
    </div>
  </div>
</template>

<script>
export default {
  name: "Store",
  props: {
    name: String,
    description: String,
    location: String,
    isOnline: Boolean
  }
};
</script>

<style>
.card-footer {
  margin-top: auto;
}
</style>
