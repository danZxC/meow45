<template> 
<h2 >Reaction time {{ score }} ms</h2>
<p>{{ rank }}</p>
</template>

<script>
export default {
    props:['score'],
    data(){
        return{
            rank: null,
        }
    },
    mounted(){
        if(this.score<450){this.rank = 'You are fast'}
        else if(this.score <600){this.rank = "Ok"}
        else if(this.score <800){this.rank = "Not OK"}
        else{this.rank = "Br WTFFFFF"}
    },
    methods: {

    }
}
</script>

<style scoped>
h2{
    color: pink;
  font-family: Jura;
  font-size: 30px;
  font-style: normal;
  font-weight: 600;
  line-height: normal;
  letter-spacing: 6px;
}
p{
    color: pink;
  font-family: Jura;
  font-size: 20px;
  font-style: normal;
  font-weight: 600;
  line-height: normal;
  letter-spacing: 6px;
}
</style>