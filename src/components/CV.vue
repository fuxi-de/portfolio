<template>
  <div class="cv">
    <div class="inner-wrapper">
      <p class="intro">This is where I have worked so far:</p>
      <Table :parentData="jobs" />
    </div>
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
        {
          employer: "Bauer Xcel Media",
          location: "Hamburg",
          position: "Software Engineer",
          date: "10.2018 - today"
        },
        {
          employer: "Schumacher Brand + Interaction Design",
          location: "Darmstadt",
          position: "Web Developer",
          date: "11.2017 - 10.2018"
        },
        {
          employer: "Quäntchen + Glück",
          location: "Darmstadt",
          position: "Web Developer",
          date: "06.2016 - 10.2017"
        },
        {
          employer: "Selfemployed",
          location: "Darmstadt, Mainz",
          position: "Web Developer",
          date: "10.2014 - 05.2016"
        },
        {
          employer: "Surfer's Paradise",
          location: "Fehmarn",
          position: "Windsurf- & Kiteinstructor",
          date: "05.2014 - 10.2014"
        },
        {
          employer: "Havas Media Group",
          location: "Frankfurt",
          position: "Working Student",
          date: "06.2012 - 05.2014"
        }
      ]
    }
  },
  methods: {}
}
</script>

<style lang="scss">
.cv {
  .inner-wrapper {
    max-width: 75%;
    margin: auto;
  }
  .intro {
    width: 50%;
    text-align: center;
    font-family: "Red Hat Display", sans-serif;
    font-size: 1.5em;
    margin: auto;
    margin-bottom: 50px;
  }
  margin: auto;
  background: white;
  padding-bottom:100px;
}
</style>