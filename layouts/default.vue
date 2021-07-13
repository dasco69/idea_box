<template>
    <div class="container mx-auto px-10">
    <Navbar />
    <transition name="rotateX">
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
rotate-enter { transform: perspective(500px) rotate3d(0, 1, 0, 90deg); }
.rotate-enter-active,
.rotate-leave-active { transition: 0.5s; }
.rotate-leave-to { transform: perspective(500px) rotate3d(0, 1, 0, -90deg); }

.rotateX-enter { transform: matrix(2, 5, 5, 2, 5, 6);}
.rotateX-enter-active,
.rotateX-leave-active { transition: 0.5s; }
.rotateX-leave-to { transform: perspective(500px) rotate3d(0, 1, 0, -90deg); }
</style>
