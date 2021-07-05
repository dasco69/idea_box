<template>
  <div class="container mx-auto">
    <Navbar />
    <transition name="color" mode="out-in">
      <Nuxt />
    </transition>
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
