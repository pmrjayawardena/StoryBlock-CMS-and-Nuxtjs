<template>
  <div>
    <main class="main-content">
      <TheHeader />
      <Nuxt />
    </main>
  </div>
</template>

<script>
import TheHeader from "../components/TheHeader/TheHeader";

export default {
  components: {
    TheHeader
  }
};
</script>

<style>
* {
  box-sizing: border-box;
  padding: 0;
  margin: 0;
}
body {
  font-family: "Lato", sans-serif;
  margin: 0;
}

.main-content {
  margin-top: 4.5rem;
}
</style>
