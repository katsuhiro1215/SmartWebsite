<script setup>
</script>

<template>
  <section class="relative w-full h-[720px] flex items-center px-14">
    <div class="absolute w-1/2 h-3/5 top-1/4 right-0">
      <div class="drop absolute"></div>
      <div class="drop absolute"></div>
      <div class="drop absolute"></div>
      <div class="drop absolute"></div>
    </div>
    <div class="w-1/2 px-14 space-y-6">
      <h3 class="text-6xl font-light">Smart Sprouts System</h3>
      <p class="pl-4 text-lg">
        Lorem ipsum dolor sit amet consectetur adipisicing elit. Quis dolore
        saepe atque et fugiat in enim odit eos quasi voluptates.
      </p>
    </div>
  </section>
</template>

<style>
.drop {
  width: 320px;
  height: 320px;
  background: transparent;
  box-shadow: inset 10px 10px 10px rgba(0, 0, 0, 0.05),
    15px 25px 10px rgba(0, 0, 0, 0.1), 15px 20px 20px rgba(0, 0, 0, 0.05),
    inset -10px -10px 15px rgba(255, 255, 255, 0.9);
  animation: fluidrotate1 30s ease 0s infinite;
}
.drop::before {
  content: "";
  position: absolute;
  top: 75px;
  left: 80px;
  background-color: #fff;
  width: 24px;
  height: 24px;
  border-radius: 42% 58% 37% 63% / 40% 43% 57% 60%;
}
.drop::after {
  content: "";
  position: absolute;
  top: 75px;
  left: 120px;
  background: #fff;
  width: 12px;
  height: 12px;
  border-radius: 57% 43% 37% 63% / 48% 37% 63% 52%;
}
.drop:nth-child(2) {
  transform: scale(0.5) translate(-500px, 180px);
  animation: fluidrotate2 30s ease 0s infinite;
}
.drop:nth-child(3) {
  transform: scale(0.5) translate(500px, 10px);
  animation: fluidrotate3 30s ease 0s infinite;
}
.drop:nth-child(4) {
  transform: scale(0.25) translate(120px, -860px);
  animation: fluidrotate4 30s ease 0s infinite;
}

@keyframes fluidrotate1 {
  0%,
  100% {
    border-radius: 63% 37% 54% 46%/55% 48% 52% 45%;
  }
  14% {
    border-radius: 40% 60% 54% 46%/49% 60% 40% 51%;
  }
  28% {
    border-radius: 54% 46% 38% 62%/49% 70% 30% 51%;
  }
  42% {
    border-radius: 61% 39% 55% 45%/61% 38% 62% 39%;
  }
  56% {
    border-radius: 61% 39% 67% 33%/70% 50% 50% 30%;
  }
  70% {
    border-radius: 50% 50% 34% 66%/56% 68% 32% 44%;
  }
  84% {
    border-radius: 46% 54% 50% 50%/35% 61% 39% 65%;
  }
}
@keyframes fluidrotate2 {
  0%,
  100% {
    border-radius: 63% 37% 54% 46%/55% 48% 52% 45%;
  }
  14% {
    border-radius: 40% 60% 54% 46%/49% 60% 40% 51%;
  }
  28% {
    border-radius: 54% 46% 38% 62%/49% 70% 30% 51%;
  }
  42% {
    border-radius: 61% 39% 55% 45%/61% 38% 62% 39%;
  }
  56% {
    border-radius: 61% 39% 67% 33%/70% 50% 50% 30%;
  }
  70% {
    border-radius: 50% 50% 34% 66%/56% 68% 32% 44%;
  }
  84% {
    border-radius: 46% 54% 50% 50%/35% 61% 39% 65%;
  }
}
@keyframes fluidrotate3 {
  0%,
  100% {
    border-radius: 63% 37% 54% 46%/55% 48% 52% 45%;
  }
  14% {
    border-radius: 40% 60% 54% 46%/49% 60% 40% 51%;
  }
  28% {
    border-radius: 54% 46% 38% 62%/49% 70% 30% 51%;
  }
  42% {
    border-radius: 61% 39% 55% 45%/61% 38% 62% 39%;
  }
  56% {
    border-radius: 61% 39% 67% 33%/70% 50% 50% 30%;
  }
  70% {
    border-radius: 50% 50% 34% 66%/56% 68% 32% 44%;
  }
  84% {
    border-radius: 46% 54% 50% 50%/35% 61% 39% 65%;
  }
}
@keyframes fluidrotate4 {
  0%,
  100% {
    border-radius: 63% 37% 54% 46%/55% 48% 52% 45%;
  }
  14% {
    border-radius: 40% 60% 54% 46%/49% 60% 40% 51%;
  }
  28% {
    border-radius: 54% 46% 38% 62%/49% 70% 30% 51%;
  }
  42% {
    border-radius: 61% 39% 55% 45%/61% 38% 62% 39%;
  }
  56% {
    border-radius: 61% 39% 67% 33%/70% 50% 50% 30%;
  }
  70% {
    border-radius: 50% 50% 34% 66%/56% 68% 32% 44%;
  }
  84% {
    border-radius: 46% 54% 50% 50%/35% 61% 39% 65%;
  }
}
</style>