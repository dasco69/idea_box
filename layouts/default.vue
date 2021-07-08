<template>
  <div class="container mx-auto">
    <Navbar />
    <Nuxt />
  </div>
</template>
<style>

.fade-enter-active, .fade-leave-active {
  transition: opacity 0.25s ease-out;
}

.fade-enter, .fade-leave-to {
  transform: translateX(100%);
}
</style>
