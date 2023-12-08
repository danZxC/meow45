<script setup>
import first from './components/first-screen.vue'
import second from './components/second-screen.vue'
import third from './components/third-screen.vue'
import fourth from './components/fourth-screen.vue'
import contacts from './components/contacts.vue'
</script>


<template>
  <first/>
  <second/>
  <third/>
  <fourth/>
  <contacts/>
</template>

<script>
export default {
  components: {first,second, third, fourth, contacts},
}
</script>

<style >
@import url('https://fonts.googleapis.com/css2?family=Jura&family=Manrope:wght@600&family=Nunito&display=swap');

#app {
  padding:0;
  margin: 0;
  text-align: center;
  display: flex;
  flex-direction: column;
  align-items: center;
}
</style>
