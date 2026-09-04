<script setup lang="ts">
</script>

<template>
  <div class="home-view">
    <h1>RIGEL S.A.</h1>
    <p>rigel-frontapp listo para trabajar</p>
  </div>
</template>

<style lang="scss" scoped>
.home-view {
  display: flex;
  flex-direction: column;
  align-items: center;
  justify-content: center;
  min-height: 100vh;
  gap: 1rem;

  h1 {
    font-family: $font-principal;
    font-size: 2.5rem;
    font-weight: 700;
    color: $primary;
  }

  p {
    font-family: $font-principal;
    font-size: 1.2rem;
    color: $text-secondary;
  }
}
</style>
