<template>
  <div class="table">
    <div v-for="item in parentData" class="table-element">
      <div v-for="(value, name) in item" class="row">
        <div class="table-element-header">{{ name }}</div>
        <div class="table-element-content">{{ value }}</div>
      </div>
    </div>
  </div>
</template>

<script>
export default {
  name: "Table",
  props: ["parentData"],
  methods: {}
}
</script>

<style lang="scss">
.table-element {
  font-family: "Red Hat Display", sans-serif;
  .row {
    display: grid;
    grid-template-columns: 1fr 1fr;
  }
  &-header {
    font-size: 1.3em;
    font-weight: bold;
    text-align: right;
    padding: 15px;
  }
  &-content {
    font-size: 1.3em;
    font-weight: lighter;
    padding: 15px;
  }
}
</style>