<template>
  <div class="keyvisual">
    <!-- <g-image src="~/images/tracy-adams.jpg" width="500"/> -->
    <div class="intro">
      <span class="greeting">
        Hi, my Name is
        <span class="name">{{ name }}</span>
        !
      </span>
      <span class="about">{{ about }}</span>
    </div>
    <button @click="onClick">Change</button>
  </div>
</template>

<script>
export default {
  name: "Keyvisual",
  data() {
    return {
      name: "Flo",
      about:
        "I am a Fullstack Webdeveloper currently living and working in Hamburg, Germany"
    }
  },
  methods: {
    onClick() {
      this.name = "Here you go :)"
    }
  }
}
</script>

<style lang="scss">
.keyvisual {
  min-height: 100vh;
  display: flex;
  align-items: center;
  justify-content: center;
  position:fixed;
  top:0;
  bottom:0;
  left:0;
  right:0;
  z-index:-1;
  .greeting {
    font-family: "Lacquer", sans-serif;
    font-size: 4em;
    display: block;
    text-align: center;
    .name {
      text-decoration: underline;
      text-decoration-color: #725ac1;
    }
  }
  .about {
    font-family: "Lacquer", sans-serif;
    font-size: 1.5em;
    display: block;
    text-align: center;
  }
}
</style>