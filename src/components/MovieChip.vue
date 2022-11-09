<script setup>
console.log("test");
</script>
<template>
  <div class="movie-chip"><slot></slot></div>
</template>
<style scoped>
.movie-chip {
  background: #9b59b6;
  float: left;
  padding: 6px 12px;
  border-radius: 30px;
  color: #fff;
  margin-right: 8px;
  opacity: 0;
  animation: fadeUpIn ease-in 0.1s 1 forwards;
}

@keyframes fadeUpIn {
  0% {
    transform: translateY(10px);
  }

  50% {
    transform: translateY(-5px);
  }

  100% {
    opacity: 1;
    transform: translateY(0);
  }
}
</style>
