<template>
  <div class="columns is-mobile">
    <div class="column">
      <div class="control has-icons-left">
        <input class="input" type="text" placeholder="Search products">
        <span class="icon is-left">
          <b-icon icon="magnify" size="is-small"></b-icon>
        </span>
      </div>
    </div>
    <div class="column is-narrow">
      <div class="select">
        <select>
          <option>Grocery</option>
          <option>Books</option>
          <option>Electronics</option>
          <option>Entertainment</option>
        </select>
      </div>
    </div>
  </div>
</template>

<script>
export default {
  name: "Search"
};
</script>
