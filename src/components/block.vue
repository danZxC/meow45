<template>
    <div class="block" v-if="showBlock" @click = "stopTimer">
        click me
    </div>
</template>


<script>
export default{
    props: ['delay'],
    data(){
        return{
            showBlock: false,
            timer: null,
            reactionTime:0
        }
    },
    mounted(){
        setTimeout(()=> {
            this.showBlock=true
            this.startTimer()
        },this.delay)
    },
    methods: {
        startTimer(){
            this.timer=setInterval(()=> {
                this.reactionTime += 10
            })
        },
        stopTimer(){
            clearInterval(this.timer)
            this.$emit('end', this.reactionTime)
        }
    }
}
</script>


<style scoped>
    .block {
        font-size: 100px;
        display: flex;
        justify-content: center;
        align-items: center;
        width: 70%;
        height: 30%;
        background-image: url('../assets/texture.png');
        background-size: cover;
        color:white;
        text-align: center;
        padding: 100px;
        margin: 40px auto;
    }

    @media (max-width: 1440px){

        .block{
            width: 100%;
            font-size: calc(30px + 10 * (100vw / 1280));
        }
    }
    @media (max-width: 440px){
        .block{
            height: 20%;
        }
    }
</style>

<style>

</style>

