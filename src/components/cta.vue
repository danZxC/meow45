<template>
    <div class="wrapper">        
      
        <h1>KANBAN</h1>
        <h2>Через тернии к эффективности</h2>
        <button > <a href="https://kkkiska.github.io/gmrpo/">Перейти к доске</a></button>
    </div>
</template>


<script>

</script>


<style scoped>
.wrapper {
    width: 60%;
    height: 60%;
    margin-top: 170px;
    display: flex;
    flex-direction: column;
    align-items: center;
    justify-content: space-between;
}
h1 {
     display: inline;
    font-family: 'Jura',sans-serif;
    font-size: 200px;
    color:white;
    letter-spacing: 40px;
    border-radius: 40px;
    padding: 20px 60px;
    font-weight: 300;
    background-image:url('../assets/texture.png') ;

}
h2 {
    color: #1B338D;
    font-family: Overpass;
    font-size: 30px;
    font-style: normal;
    font-weight: 300;
    line-height: normal;
    letter-spacing: 5.4px;
}

button{
    color: #1B338D;
    font-family: Jura;
    font-size: 35px;
    font-style: normal;
    font-weight: 600;
    line-height: normal;
    letter-spacing: 6.3px;
    background-image: url('../assets/bg-second.png');
    height: 20%;
    width: 50%;
    border-radius: 30px;
    background-size: cover;
    border:0

}

a {
  text-decoration: none;
  color:white;
}
a:visited{
  text-decoration: none;
  color:white;
}

@media (max-width: 1440px){
  .wrapper {
    background-color: white;
    background-image: none;
  }
  h1{
    font-size: calc(30px + 20 * (100vw / 1280));
  }
  button {
    font-size: calc(16px + 10 * (100vw / 1280));
    
  }
  .wrapper{
    height: 40%;
  }
}

@media (max-width: 768px){
  .wrapper{
    position: relative;
    height: 30%;
    margin-top: 100px;
  }
  h1{
    font-size: calc(20px + 20 * (100vw / 1280));
  }
  button{
    width: 100%;
    font-size: calc(10px + 10 * (100vw / 1280));
  }
}

@media (max-width:480px){
  h1{
    padding: 20px 10px;
    background-size: cover;
  }
  button{
    width: 100%;
  }
  h2{
    font-size: calc(15px + 15 * (100vw / 1280));
  }
}
</style>

<style>
/* Указываем box sizing */
*,
*::before,
*::after {
  box-sizing: border-box;
}

/* Убираем внутренние отступы */
ul[class],
ol[class] {
  padding: 0;
}

/* Убираем внешние отступы */
body,
h1,
h2,
h3,
h4,
p,
ul[class],
ol[class],
li,
figure,
figcaption,
blockquote,
dl,
dd {
  margin: 0;
}

/* Выставляем основные настройки по-умолчанию для body */
body {
  min-height: 100vh;
  scroll-behavior: smooth;
  text-rendering: optimizeSpeed;
  line-height: 1.5;
}

/* Удаляем стандартную стилизацию для всех ul и il, у которых есть атрибут class*/
ul[class],
ol[class] {
  list-style: none;
}

/* Элементы a, у которых нет класса, сбрасываем до дефолтных стилей */
a:not([class]) {
  text-decoration-skip-ink: auto;
}

/* Упрощаем работу с изображениями */
img {
  max-width: 100%;
  display: block;
}

/* Указываем понятную периодичность в потоке данных у article*/
article > * + * {
  margin-top: 1em;
}

/* Наследуем шрифты для инпутов и кнопок */
input,
button,
textarea,
select {
  font: inherit;
}

/* Удаляем все анимации и переходы для людей, которые предпочитай их не использовать */
@media (prefers-reduced-motion: reduce) {
  * {
    animation-duration: 0.01ms !important;
    animation-iteration-count: 1 !important;
    transition-duration: 0.01ms !important;
    scroll-behavior: auto !important;
  }
}
</style>