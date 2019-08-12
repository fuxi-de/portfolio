<template>
  <div class="table">
    <div v-for="item in parentData" class="row">
      <div>header</div>
      <div>{{ item.employer }}</div>
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
.table {
  .row {
    display: grid;
    grid-template-columns: 1fr 1fr;
  }
}
</style>