<template>
  <img class="NuxtLogo" src="bird.png" />
</template>
<style>
.NuxtLogo {
  animation: 5s appear;
  border-radius: 50%;
}

@keyframes appear {
  0% {
    opacity: 0;
  }
  100% {
    opacity: 1;
  }
}
</style>
