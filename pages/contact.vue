<template>
  <div class="about">
    <h1>Contact</h1>
    <p>
        this will be a form
    </p>
  </div>
</template>

<script>
export default {
  
};
</script>

<style lang="scss" scoped>

.page-enter-active {
  animation: acrossIn .40s ease-out both;
} 

.page-leave-active {
  animation: acrossOut .60s ease-in both;
} 
@keyframes acrossIn {
0% {
  transform: translate3d(-100%, 0, 0);
  opacity: 0;
}
100% {
  transform: translate3d(0, 0, 0);
  opacity: 100%;
}
}
@keyframes acrossOut {
0% {
  transform: translate3d(0, 0, 0);
  opacity: 100%;
}
100% {
  transform: translate3d(-100%, 0, 0);
  opacity: 0;
}
}
.about {
  margin: 30px auto 50px;
  max-width: 800px;
  padding: 50px 50px 70px;
  background: white;
}

p {
  margin: 15px 0 20px;
}
</style>