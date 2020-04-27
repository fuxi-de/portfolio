<template>
  <div class="footer h-40 flex flex-col items-center justify-center text-xl">
    <span>© {{ new Date().getFullYear() }} Florian Schildwächter</span>
    <a target="_blank" href="https://icons8.com">Favicon by Icons8</a>
  </div>
</template>

<script>
export default {
  name: "Footer",
  data() {
    return {};
  },
};
</script>

<style lang="scss">
.footer {
  box-shadow: 0 -24px 24px rgba(150, 150, 150, 0.22);
  width: 100%;
  background: #3f4045;
  color: white;
  font-family: "Red Hat Display", sans-serif;
}
</style>
