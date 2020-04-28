<template>
  <div class="aboutme">
    <div class="md:w-9/12 mb-32 mt-40 flex flex-col md:flex-row items-center justify-around">
      <p class="w-11/12 md:w-1/2 mb-16">{{ aboutMe }}</p>
      <g-image src="~/assets/kitesurfing.svg" width="350" />
    </div>
    <p class="w-11/12 text-center mb-8">
      This is a small (incomplete) list of technologies i've enjoyed working with:
    </p>
    <ul class="techlist mb-48 flex flex-row flex-wrap w-9/12 justify-center">
      <li class="m-2" v-for="(item, index) in iLike" :key="index">
        {{ item }}
      </li>
    </ul>
    <div class="w-9/12 mb-32 flex flex-col md:flex-row items-center justify-around">
      <g-image class="mb-16 md:mb-0" src="~/assets/networking.svg" width="350" />
      <div>
        <p>follow me on these platforms if you like:</p>
        <ul class="linklist">
          <li v-for="(link, index) in links" :key="index">
            <a :href="link.target" target="blank">{{ link.name }}</a>
          </li>
        </ul>
      </div>
    </div>
  </div>
</template>

<script>
export default {
  name: "AboutMe",
  data() {
    return {
      aboutMe:
        "I am 27 years of age and was born in the ruhrgebiet area. My passion is tinkering around with code and ideally creating value throughout the whole development lifecycle. I highly believe in finding and using the right tool for the job rather then relying on the same set of tools for all purposes. In my freetime I am also flying kites at the german shores!",
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
        "git",
      ],
      links: [
        {
          name: "github",
          target: "https://github.com/fuxi-de"
        },
        {
          name: "linkedin",
          target: "https://www.linkedin.com/in/florian-schildwaechter/"
        },
        {
          name: "stackoverflow",
          target: "https://stackoverflow.com/users/story/10996848"
        },
        {
          name: "twitter",
          target:"https://twitter.com/Fuxifuchsi"
        }
      ],
    };
  },
  methods: {},
};
</script>

<style lang="scss">
.aboutme {
  min-height: 100vh;
  margin-top: 100vh;
  background: white;
  box-shadow: 0 -24px 24px rgba(150, 150, 150, 0.22);
  font-family: "Red Hat Display", sans-serif;
  font-size: 1.5em;
  display: flex;
  flex-direction: column;
  align-items: center;
  justify-content: center;
  .techlist {
    list-style: none;
    li {
      padding-left: 10px;
      padding-right: 10px;
      border-radius: 4%;
      background: #725ac1;
      color: white;
      text-align: center;
    }
  }
  .linklist {
    list-style: none;
    li {
      text-decoration: underline;
      color: #725ac1;
    }
  }
}
</style>
