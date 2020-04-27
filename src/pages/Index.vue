<template>
  <Layout>
    <Keyvisual />
    <AboutMe />
    <CV />
    <Footer />
  </Layout>
</template>

<script>
import Keyvisual from "~/components/Keyvisual"
import CV from "~/components/CV"
import AboutMe from "~/components/AboutMe"
import Footer from "~/components/Footer"

export default {
  metaInfo: {
    title: "Moin, world!"
  },
  components: {
    Keyvisual,
    CV,
    AboutMe,
    Footer
  }
}
</script>

<style>
</style>
