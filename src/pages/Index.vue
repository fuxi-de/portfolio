<template>
  <Layout>
    <Keyvisual />
    <AboutMe />
    <CV />
  </Layout>
</template>

<script>
import Keyvisual from "~/components/Keyvisual"
import CV from "~/components/CV"
import AboutMe from "~/components/AboutMe"

export default {
  metaInfo: {
    title: "Hello, world!"
  },
  components: {
    Keyvisual,
    CV,
    AboutMe
  }
}
</script>

<style>
.home-links a {
  margin-right: 1rem;
}
</style>
