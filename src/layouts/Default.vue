<template>
  <div class="layout">
    <!-- <header class="header">
      <strong>
        <g-link to="/">{{ $static.metaData.siteName }}</g-link>
      </strong>
      <nav class="nav">
        <g-link class="nav__link" to="/">Home</g-link>
        <g-link class="nav__link" to="/about">About</g-link>
      </nav>
    </header>-->
    <slot />
  </div>
</template>

<static-query>
query {
  metaData {
    siteName
  }
}
</static-query>

<style lang="scss">
@font-face {
  font-family: "Press Start 2P";
  src: url("../assets/fonts/Press_Start_2P/PressStart2P-Regular.ttf");
  font-weight: normal;
}
@font-face {
  font-family: "Red Hat Display";
  src: url("../assets/fonts/Red_Hat_Display/RedHatDisplay-Regular.ttf");
  font-weight: normal;
}

body {
  font-family: -apple-system, system-ui, BlinkMacSystemFont, "Segoe UI", Roboto,
    "Helvetica Neue", Arial, sans-serif;
  margin: 0;
  padding: 0;
  line-height: 1.5;
}

.layout {
  max-width: 100%;
  margin: 0 auto;
}

.header {
  display: flex;
  justify-content: space-between;
  align-items: center;
  margin-bottom: 20px;
  height: 80px;
  .nav__link {
    margin-left: 20px;
  }
}
</style>
