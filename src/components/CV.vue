<template>
  <div class="cv">
    <Table :parentData="jobs" />
  </div>
</template>

<script>
import Table from "~/components/Table"
export default {
  name: "CV",
  components: {
    Table
  },
  data() {
    return {
      jobs: [
        { employer: 'havas', date: 2017 }
      ]
    }
  },
  methods: {}
}
</script>

<style lang="scss">
.cv {
  max-width: 75%;
  margin:auto;
}
</style>