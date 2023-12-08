<template>
    <div class="burger" @click="show" >
        <div class="burger-part"></div>
        <div class="burger-part"></div>
        <div class="burger-part"></div>
    </div>
    <ul class="nav-list" v-if="showMenu==true">
        <li><a href="#">Главная</a></li>
        <li><a href="https://kkkiska.github.io/gmrpo/">Доска</a></li>
        <li><a href="https://danzxc.github.io/meou/">О нас</a></li>
        <li><a href="#">Контакты</a></li>
    </ul>
</template>

<script>
       export default {
        data(){
            return{
                showMenu: true
            }
        },
        methods: {
            show(){
                this.showMenu=!this.showMenu
            }
        }
       }

</script>

<style scoped>
.burger{
    display:flex;
    flex-direction: column;
    justify-content: space-between;
    width: 100px;
    height: 100px;
    display: none;
}
.burger-part {
    display: block;
    width: 100%;
    background-color: #1B338D;
    height: 15%;
}
ul {
    margin:0 auto;
    list-style: none;
    color: black;
    display: flex;
    width: 40%;
    justify-content: space-between;
    align-items: center;
    z-index: 100;
}
li{margin-top:30px}
li a{
    padding:20px 40px;
    box-sizing: border-box;
    text-decoration: none;
}
li a:hover{

    border-bottom: 5px solid #1B338D;
}
a:visited{
    color:black;
}

@media (max-width: 1440px){
    ul {
        width: 70%;
    }
    li a {
        font-size: calc(8px + 8 * (100vw / 1280));
    }
}
@media (max-width:768px){
    .burger{
        display: flex;
        margin-top: 30px;
        margin-left: 70%;
        padding-bottom: 12px;
        width: 40px;
        height: 40px;
        color:#1B338D;
    }
    .burger-part{
        width: 100%;
        height: 25%;
    }
    ul{
        display: flex;
        flex-direction: column;
        justify-content: space-between;
    }
    
}
</style>

