<template>
  <div class="keyvisual">
    <div class="intro">
      <div class="flex flex-row items-center justify-center">
        <span class="greeting m-2 text-6xl self-end">
          Hi, my Name is
          <span class="name">{{ name }}</span>
          !
        </span>
        <g-image class="m-2" src="~/assets/flo.svg" width="300" />
      </div>
      <span class="about text-3xl">{{ about }}</span>
    </div>
  </div>
</template>

<script>
export default {
  name: "Keyvisual",
  data() {
    return {
      name: "Flo",
      about:
        "I am a Software Engineer currently living and working in Hamburg, Germany",
    };
  },
};
</script>

<style lang="scss">
.keyvisual {
  min-height: 100vh;
  display: flex;
  align-items: center;
  justify-content: center;
  position: fixed;
  top: 0;
  bottom: 0;
  left: 0;
  right: 0;
  z-index: -1;
  .greeting {
    font-family: "Lacquer", sans-serif;
    display: block;
    text-align: center;
    .name {
      text-decoration: underline;
      text-decoration-color: #725ac1;
    }
  }
  .about {
    font-family: "Lacquer", sans-serif;
    display: block;
    text-align: center;
  }
}
</style>
