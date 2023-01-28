<script>

import NavContent from './NavContent.vue';

export default {

    name: "AppHeader",

    data() {
        return {

            currentLink: 0,
            showMenu: false,

            linksInfo: [
                {
                    linkName: "HOME",
                    linkRef: "#",
                    id: 0
                },
                {
                    linkName: "SERVIZI",
                    linkRef: "#",
                    id: 1
                },
                {
                    linkName: "LAVORI",
                    linkRef: "#",
                    id: 2
                },
                {
                    linkName: "CHI SIAMO",
                    linkRef: "#",
                    id: 3
                },
                {
                    linkName: "CONTATTI",
                    linkRef: "#",
                    id: 4
                },

            ]
        }
    },
    components: {
        NavContent,
    }, 
    methods:{
        onLinkClick(i){
            this.currentLink = i;
        },
        showOffCanvasMenu(){
            this.showMenu ? this.showMenu = false : this.showMenu = true;
        }
    }
}
</script>

<template>
  
    <div class="container-fluid">
        <a href="#">
            <img class="logo" src="../../assets/img/construction_logo.png" alt="Header Logo">
        </a>
        <nav class="header-nav d-none d-lg-flex">
            <NavContent
            v-for="(linkInfo, index) in this.linksInfo" 
            :info="linkInfo" 
            :currentLink="this.currentLink"
            @onLinkClick="onLinkClick(index)" />

            <button class="nav-btn">SCOPRI DI PIU</button>
        </nav>
        <nav class="burger-menu d-lg-none d-md-flex">

            <div class="dropdown">
                <button class="btn" type="button" data-bs-toggle="dropdown" aria-expanded="false" @click.prevent="showOffCanvasMenu()">
                    <i class="fa-solid fa-bars burger-menu-icon"></i>
                </button>
                <ul class="dropdown-menu" :class="showMenu ? 'show' : ''" tabindex="-1" :style="{ visibility: showMenu ? 'visible' : 'hidden' }">
                    <li class="burger-item">
                        <a class="dropdown-item" href="#">
                            <span><i class="fa-solid fa-house burger-link-icon"></i>HOME</span>
                        </a>
                    </li>
                    <li class="burger-item">
                        <a class="dropdown-item" href="#">
                            <span><i class="fa-solid fa-toolbox burger-link-icon"></i>SERVIZI</span>
                        </a>
                    </li>
                    <li class="burger-item">
                        <a class="dropdown-item" href="#">
                            <span><i class="fa-solid fa-hammer burger-link-icon"></i>LAVORI</span>
                        </a>
                    </li>
                    <li class="burger-item">
                        <a class="dropdown-item" href="#">
                            <span><i class="fa-solid fa-users burger-link-icon"></i>CHI SIAMO</span>
                        </a>
                    </li>
                    <li class="burger-item">
                        <a class="dropdown-item" href="#">
                            <span><i class="fa-sharp fa-solid fa-phone-volume burger-link-icon"></i>CONTATTI</span>
                        </a>
                    </li>
                </ul>
            </div>

        </nav>
    </div>

</template>

<style scoped>

.container-fluid{
    display: flex;
    justify-content: space-between;
    align-items: center;
    padding: .9375rem 3.125rem;
}

.header-nav{
    display: flex;
    align-items: center;
}

.logo{
    max-width: 9.375rem;
    max-height: 9.375rem;
}

.nav-btn{
    color: gray;
    background-color: var(--first-color);
    border: none;
    padding: .4375rem .9375rem;
    margin-left: .3125rem;
    cursor: pointer;
}

.nav-btn:hover{
    color: white;
    background-color: var(--second-color);
}

.burger-menu{
    display: flex;
    align-items: center;
}

.burger-menu-icon{
    color: var(--second-color);
    font-size: 1.875rem;
    padding: 0 .625rem;
}

.burger-link-icon{
    margin-right: .3125rem;
}

.burger-link-icon-special{
    margin-right: .5rem;
}

.burger-special-text{
    margin-left: .3125rem;
}

.dropdown{
    position: relative;
}

.dropdown-menu{
    position: absolute;
    right: 26%;
}

.dropdown-item{
    text-align: start;
}

</style>