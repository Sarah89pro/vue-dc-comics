<template>
<header class="container">
    <div class="img">
        <img src="../assets/img/dc-logo.png" alt="">
    </div>
    <div class="menu">
        <ul>
            <li
            v-for="(link, index) in links"
            :key="index" :class="{active: link.active}" >
            <a
            :class="{selected: link.active}"
            :href="link.url">{{ link.nome }}
            </a>
            </li>
        </ul>
    </div>
</header>
</template>

<script>
export default {
    name: 'Header',
    data() {
        return {
            links: [
                {
                    nome: 'characters',
                    url: '/characters',
                    active: true
                },
                { 
                    nome: 'comics',
                    url: '/comics',
                    active: false
                },
                { 
                    nome: 'movies',
                    url: '/movies',
                    active: false
                },
                {
                    nome: 'tv',
                    url: '/tv',
                    active: false
                },
                {
                    nome: 'games',
                    url: '/games',
                    active: false
                },
                { 
                    nome: 'collectibles',
                    url: '/collectibles',
                    active: false
                },
                { 
                    nome: 'videos',
                    url: '/videos',
                    active: false
                },
                { 
                    nome: 'fans',
                    url: '/fans',
                    active: false
                },
                { 
                    nome: 'news',
                    url: '/news',
                    active: false
                },
                { 
                    nome: 'shop',
                    url: '/shop',
                    active: false
                },
            ],
        };
    },
}
</script>

<style scoped>

header {
    display: flex;
    justify-content: space-between;
    line-height: 120px;
    text-transform: uppercase;
    font-weight: bold;
    font-size: 12px;
}


a {
    color: #000;
}


.menu ul {
    display: flex;
    justify-content: center;
}


.menu li {
    margin-left: 20px;
}


.selected {
    color: rgb(45, 143, 241);
}


.active {
    border-bottom: 5px solid rgb(45, 143, 241);
}


.img {
    display: flex;
    align-items: center;
}


.img img  {
    max-width: 80px;
}
</style>