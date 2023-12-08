<template>
    <footer>
        <div class="contacts-list" id="contacts">
            <div class="contacts-item">
                <div class="contacts-item-title">Телефоны</div>
                <div class="contacts-text">+375 (29) 253-75-23</div>
                <div class="contacts-text">+375 (29) 253-75-23</div>
                <div class="contacts-text">+375 (29) 253-75-23</div>
                <div class="contacts-text">+375 (29) 253-75-23</div>
            </div>
            <div class="contacts-item">
                <div class="contacts-item-title">Instagram</div>
                <a class="contacts-text" href="https://www.instagram.com/dinka.gr/">dinka.gr</a>
                <a class="contacts-text" href="https://www.instagram.com/pz.zzz/">pz.zzz</a>
                <a class="contacts-text" href="https://www.instagram.com/daniil_kozlovzc/">daniil_kozlovzc</a>
                <a class="contacts-text" href="https://www.instagram.com/abr_katherine/">abr_katherine</a>
            </div>
        </div>
    </footer>
</template>

<style scoped>
    .contacts-list {
        
    color: #FFF;
    padding: 50px 0;
    width: 80%;
    margin: 0 auto;
    display: flex;
    flex-wrap: wrap;
    align-items: center;
    justify-content: space-evenly;
}

.contacts-item {
    padding: 20px;
    text-align: center;
}

.contacts-item-title {
    font-family: 'Caveat', cursive;
    font-size: 45px;
    font-weight: 400;
    line-height: normal;
    margin-bottom: 20px;
}

.contacts-text, a.contacts-text {
    font-family: 'Nunito Sans', sans-serif;
    font-size: 25px;
    font-weight: 300;
    line-height: normal;
    color: #FFF;
    text-decoration: none;
    display: block;
    transition: color 0.3s ease-in-out;
}

.contacts-text:hover, a.contacts-text:hover {
    color: #90CAF9; /* Light blue color for hover effect */
}

footer {
    width: 100%;
    background-color: #a2459a;
    position: relative;
}
</style>