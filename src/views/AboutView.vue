<script setup>
import CustomHeader from "../components/common/header.vue"
</script>
<template>
  <div class="about">
    <CustomHeader />
    <h1>This is an about page</h1>
  </div>
</template>

<style>
@media (min-width: 1024px) {
  .about {
    min-height: 100vh;
    display: flex;
    align-items: center;
  }
}
</style>
