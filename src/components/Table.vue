<template>
  <div class="table m-auto">
    <div v-for="(item, index) in parentData" v-bind:key="index" class="table-element">
      <div v-for="(value, name) in item" v-bind:key="name" class="row">
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
  padding-bottom: 50px;
  .row {
    display: grid;
    grid-template-columns: 1fr 1.1fr;
  }
  &-header {
    font-size: 1.3em;
    font-weight: bold;
    text-align: right;
    padding: 10px;
    color: #725ac1;
  }
  &-content {
    font-size: 1.3em;
    font-weight: lighter;
    padding: 10px;
  }
}
</style>