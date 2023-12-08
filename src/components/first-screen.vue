<script setup>
import Header from './header.vue'
import cta from './cta.vue'
</script>


<template>
  <div class="first-screen">
    <Header/>
    <cta/>
  </div>
</template>

<script>
export default {
  components: {Header, cta},
}
</script>

<style scoped>
.first-screen{
  width: 100%;
  height: 950px;
  margin: 0;
  padding: 0;
  display: flex;
  flex-direction: column;
  align-items: center;
  background-image: url('../assets/bg-first.png');
  background-repeat: no-repeat;
  background-size: cover;
}

@media (max-width: 1440px){
  .first-screen{
    background-color: white;
    background-image: none;
  }
}
</style>