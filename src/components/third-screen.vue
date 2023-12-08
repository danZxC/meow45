<template>
    <div class="third-screen">
        <div class="block-wrapper">
            <div class="block-row">
                <div class="block1">
                    <img src="../assets/icon-1.png" alt="" class="block-icon">
                    <div class="block-text">
                        <h1>Системный подход</h1>
                        <h2>
                            Рассмотрение процесса как части общей системы и учет влияния изменений в одной части на другие. Это помогает оптимизировать всю систему, а не только отдельные компоненты.
                        </h2>
                    </div>
                </div>
                <div class="block2">
                    <img src="../assets/icon-2.png" alt="" class="block-icon">
                    <div class="block-text">
                        <h1>Постоянные улучшения</h1>
                        <h2>
                            Внесение постоянных изменений и улучшений в процесс на основе накопленного опыта и обратной связи. Это обеспечивает постоянное развитие и совершенствование метода.
                        </h2>
                    </div>
                </div>
            </div>

            <div class="block-row">
                <div class="block2">
                    <img src="../assets/icon-3.png" alt="" class="block-icon">
                    <div class="block-text">
                        <h1>Визуализация процесса</h1>
                        <h2>
                            Задачи и рабочие элементы представляются в виде визуальной доски, где каждая колонка представляет определенный этап выполнения задачи. 
                        </h2>
                    </div>
                </div>
                <div class="block1">
                    <img src="../assets/icon-4.png" alt="" class="block-icon">
                    <div class="block-text">
                        <h1>Привлечение всех участников</h1>
                        <h2>
                            Активное участие всех участников процесса в его управлении и постоянное взаимодействие между участниками для совместной работы над улучшением процессов.
                        </h2>
                    </div>
                </div>
            </div>
        </div>
    </div>
</template>
    
    
    
<style scoped>
    .third-screen{
        width: 100%;
        height: 950px;
        margin: 0;
        padding: 0;
        display: flex;
        align-items: center;
        justify-content: center;
    }
    .block-wrapper {
        width: 90%;
        height: 90%;
        display: flex;
        justify-content: space-between;
        flex-direction: column;
    }
    .block-row{
        width: 100%;
        height: 45%;
        display: flex;
        justify-content:space-between;
    }

    .block1,.block2{
        width: 48%; 
        border-radius: 30px;
        display: flex;
        justify-content: space-evenly;
        align-items: center;

    }
    .block1{
        background-color: #FFF;
        filter: drop-shadow(-4px -4px 10px rgba(0, 0, 0, 0.25)) drop-shadow(4px 4px 10px rgba(0, 0, 0, 0.25));
    }
    .block2{
        background-color: #00185F;
    }

    .block-icon {
        width: 115px;
        height: 115px;
        flex-shrink: 0;
    }

    .block-text{
        text-align: left;
        width: 50%;
        height: 60%;
        display: flex;
        justify-content: space-between;
        align-items: start;
        flex-direction: column;
    }
    h1 {
        color: #00185F;
        font-family: Jura;
        font-size: 30px;
        font-style: normal;
        font-weight: 600;
        line-height: normal;
        letter-spacing: 6px;
    }

    h2{
        color: #000;
        font-family: Overpass;
        font-size: 23px;
        font-style: normal;
        font-weight: 300;
        line-height: normal;
    }

    .block2 h1{color:white}
    .block2 h2{color:white}

    @media (max-width: 1440px){
        h2{
            font-size: calc(10px + 10 * (100vw / 1280));
            
        }
        .block1,.block2{
            
            flex-direction: column;
            justify-content: space-evenly;
            align-items: center;
        }
        .block-text{
            height: 60%;
            width: 80%;
            text-align: center;
            justify-content: space-evenly;
        }
        .block-icon{
            height: 30%;
        }
        .box-wrapper{
            height: 100%;
        }
        h1{font-size: calc(16px + 16 * (100vw / 1280));}
    }

    @media (max-width: 768px){
        .block-row{
            flex-direction: column;
            justify-content: space-between;
            align-items: center;
            gap:5%;
        }
        .block-wrapper{
            gap:5%;
            justify-content: center;
            height: 100%;
        }
        .block1,.block2{
            width: 80%;
            height: 60%;
        }

        .third-screen{
            height: 2000px;
        }
        .block-icon{
            height: 20%;
            width: 30%;
        }
    }
</style>
    