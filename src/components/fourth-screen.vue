<script setup>
import block from './block.vue'
import results from './results.vue'
</script>
<template>
    <div class="fourth-screen">
       <div class="wrapper">
        <h1>REACTION TIMER</h1>
        <block v-if="playing" :delay="delay" @end="endGame"/>
        <button @click = "start" :disabled="playing">Play</button>
        <results :score = "score" v-if="showResults"/>
       </div>
    </div>
</template>

<script>
export default {
  components: {block, results},
  data(){
    return {
      playing: false,
      delay: null,
      score:null,
      showResults:false,
    }
  },
  methods: {
    start(){
      this.delay=2000+Math.random()*5000
      this.playing=true
      this.showResults=false
    },
    endGame(reactionTime){
      this.score = reactionTime
      this.playing=false
      this.showResults=true
    }
  }
}
</script>

<style scoped>
.fourth-screen{
  background: url('../assets/bg-four.jpg');
  background-size: cover;
        background-repeat: no-repeat;
        animation: bg-animation 25s ease-in-out infinite;
  width: 100%;
  height: 950px;
  margin: 0;
  padding: 0;
  display: flex;
  flex-direction: column;
  align-items: center;
  justify-content: center;
}
.wrapper {
  display: flex;
  flex-direction: column;
  width: 50%;
  height: 60%;
  justify-content: space-between;
  align-items: center;
}
button {
    font-family: Jura;
    font-size: 35px;
    font-style: normal;
    font-weight: 600;
    line-height: normal;
    letter-spacing: 6.3px;

    height: 20%;
    width: 50%;
    border-radius: 30px;
    background-color: pink;
    color:rgb(59, 0, 59);
    background-size: cover;
    border:0;
    
}
h1 {
  color: pink;
  font-family: Jura;
  font-size: 30px;
  font-style: normal;
  font-weight: 600;
  line-height: normal;
  letter-spacing: 6px;
}
@media (max-width: 1440px){
  .fourth-screen{
    animation-play-state: paused;
    background-size: cover;
    height: 100vw;
  }
  .wrapper{
    width: 80%;
  }
}
@media (max-width:468px){
  button{
    width: 80%;
  }
}
</style>

<style>
    @keyframes bg-animation {
    0% {
        background-size: 120%;
        background-position: 50% 50%
        
    }
    20% {
        background-size: 150%;
        background-position: 0 50%;
    }    
    40% {
        background-size: 110%;
        background-position: 20% 80%;
    }
    60% {
        background-size: 160%;
        background-position: 60% 10%;
    }
    80% {
        background-size: 120%;
        background-position: 40% 70%;
    }    
    100% {
        background-size: 120%;
        background-position: 50% 50%
    }}
</style>

