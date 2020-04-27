<template>
  <div class="aboutme">
    <p class="intro">{{ aboutMe }}</p>
    <p class="mb-8">This is a small list of technologies i've enjoyed working with:</p>
    <ul class="techlist flex flex-row flex-wrap w-9/12 justify-center">
      <li class="m-2" v-for="(item, index) in iLike" v-bind:key="index">{{ item }}</li>
    </ul>
  </div>
</template>

<script>
export default {
  name: "AboutMe",
  data() {
    return {
      aboutMe:
        "I am 27 years of age and was born in the ruhrgbiet area. I like tinkering around with code and flying kites at the german shores!",
      iLike: [
        "express",
        "javascript",
        "node",
        "mongoDB",
        "docker",
        "vue",
        "scss",
        "typescript",
        "php",
        "mysql",
        "laravel",
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
    //width: 75%;
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