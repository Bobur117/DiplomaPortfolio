<template>
   <div class="nav__content-menu">
        <ul class="nav__content-list">
            <NavBarListLink v-for="link in links" :key="link.title" :link="link"/>   
        </ul>
        <div class="nav__content-menu-btn">
            <div class="nav__content-menu-btn-line">
                
            </div>
        </div>
   </div>
</template>

<script setup>
import NavBarListLink from "./NavBarListLink.vue"; 


const links = [ 
    {
        title: 'Biography',
        section: 'biography',
    },
    {
        title: 'Projects',
        section: 'projects',
    },
    {
        title: 'Contacts',
        section: 'footer',
    }
];


</script>

<style lang="scss">

.nav__content-list{
    display: flex;
    justify-content: center;
    align-items: center;
    gap: 30px;
}
.nav__content-menu{
    display: flex;
    align-items: center;
}

.nav__content-menu-btn{
    width: 20px;
    height: 20px;
    display: none;
    align-items: center;
}

.nav__content-menu-btn-line{
    width: 100%;
    height: 1px;
    background: white;
    position: relative;
}

.nav__content-menu-btn-line::before {
    
    content: '';
    width: 80%;
    height: 1px;
    background: white;
    position: absolute;
    top: -5px;
    right: 0; 
    
}
.nav__content-menu-btn-line::after {
    
    content: '';
    width: 110%;
    height: 1px;
    background: white;
    position: absolute;
    top: 5px;
    right: 0; 
    
}

</style>