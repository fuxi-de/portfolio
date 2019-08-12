<template>
  <div class="aboutme">
    <p class="intro">{{ aboutMe }}</p>
    <p>This is a small list of technologies i've worked with and liked:</p>
    <ul class="techlist">
      <li v-for="item in iLike">{{ item }}</li>
    </ul>
  </div>
</template>

<script>
export default {
  name: "AboutMe",
  data() {
    return {
      aboutMe:
        "I am 26 years of age and was born in the ruhrgbiet area. Besides playing around with code I like to kitesurf at the german shores.",
      iLike: [
        "php",
        "laravel",
        "vue",
        "scss",
        "express",
        "js",
        "node",
        "ts",
        "wordpress",
        "jenkins",
        "gitlab-ci",
        "git"
      ]
    }
  },
  methods: {}
}
</script>

<style lang="scss">
.aboutme {
  min-height: 100vh;
  margin-top:100vh;
  background:white;
  box-shadow: 0 -24px 24px rgba(150,150,150,0.22);
  font-family: "Red Hat Display", sans-serif;
  font-size: 1.5em;
  display: flex;
  flex-direction: column;
  align-items: center;
  justify-content: center;
  .intro {
    width: 50%;
    text-align: center;
  }
  .techlist {
    list-style: none;
    display: flex;
    flex-direction: row;
    justify-content: space-between;
    width: 75%;
    li {
      padding-left:10px;
      padding-right:10px;
      border-radius:4%;
      background: #725ac1;
      color: white;
      text-align: center;
    }
  }
}
</style>