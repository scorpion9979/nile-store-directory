<template>
  <div class="columns is-mobile">
    <div class="column">
      <div class="control has-icons-left has-icons-right">
        <input class="input is-medium" type="text" placeholder>
        <span class="icon is-left">
          <b-icon icon="magnify" size="is-small"></b-icon>
        </span>
      </div>
    </div>
    <div class="column is-narrow">
      <div class="dropdown">
        <div class="dropdown-trigger">
          <button class="button is-medium" aria-haspopup="true" aria-controls="dropdown-menu3">
            <span>Grocery</span>
            <span class="icon is-medium">
              <i class="fas fa-angle-down" aria-hidden="true"></i>
            </span>
          </button>
        </div>
        <div class="dropdown-menu" id="dropdown-menu3" role="menu">
          <div class="dropdown-content">
            <a href="#" class="dropdown-item">Overview</a>
            <a href="#" class="dropdown-item">Modifiers</a>
            <a href="#" class="dropdown-item">Grid</a>
            <a href="#" class="dropdown-item">Form</a>
            <a href="#" class="dropdown-item">Elements</a>
            <a href="#" class="dropdown-item">Components</a>
            <a href="#" class="dropdown-item">Layout</a>
          </div>
        </div>
      </div>
    </div>
  </div>
</template>

<script>
export default {
  name: "Search"
};
</script>
