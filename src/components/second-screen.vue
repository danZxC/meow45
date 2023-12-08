<template>
<div class="second-screen">
    <div class="text-wrapper">
        
        <h1>Что это такое?</h1>
        <p>
            В мире управления проектами Kanban представляет собой систему, направленную на оптимизацию рабочего процесса и достижение постоянного потока задач. С его помощью команды могут эффективно управлять задачами, учитывать приоритеты и реагировать на изменения, что способствует повышению производительности и качества работы.
        </p>

    </div>
</div>
</template>



<style scoped>
    .text-wrapper{
       
        width: 50%;
        height: 50%;
        display: flex;
        flex-direction: column;
        justify-content:space-between;
        align-items: center;
    }
    h1 {
        color: rgb(249, 218, 255);
        text-align: center;
        font-family: Jura;
        font-size: 80px;
        font-style: normal;
        font-weight: 300;
        line-height: normal;
        letter-spacing: 14.4px;
    }
    p{
        width: 100%;
        color: #fff;
        text-align: center;
        font-family: Overpass;
        font-size: 30px;
        font-style: normal;
        font-weight: 300;
        line-height: normal;
        letter-spacing: 5.4px;
    }


    .second-screen{
        background-image: url('../assets/bg-second.png');
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

    @media (max-width: 1440px){
        h1{
            font-size: calc(20px + 20 * (100vw / 1280));
        }
        p{
            font-size: calc(10px + 10 * (100vw / 1280));
        }
        .text-wrapper {
            height: 40%;
        }
        .second-screen{
            animation-play-state: paused;
            background-size: cover;
            height: 100vw;
        }
    }

    @media (max-width: 768px){
        h1{
            font-size: calc(20px + 20 * (100vw / 768));
            width: 80%;
        }
        .text-wrapper{
            width: 80%;
            height: 50%;
        }
        p{ font-size: calc(5px + 10 * (100vw / 1280));}
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