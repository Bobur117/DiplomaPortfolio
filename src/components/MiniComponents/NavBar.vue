<template>
    <nav class="nav" :class="{ color: scrollPosition > 0 }">
        <div class="nav__content container"> 
           <NavBarLogo /> 
           <NavBarList />
        </div>
    </nav>
  
</template>

<script setup>
import NavBarLogo from "./NavBarLogo.vue";
import NavBarList from "./NavBarList.vue";

import { ref } from "vue";
const scrollPosition = ref(0);

window.addEventListener('scroll', () => scrollPosition.value = window.scrollY);
</script>

<style lang="scss">

.nav{
    background: rgba(20, 20, 20, 0.50);
    border-bottom: 1px solid rgba(255, 255, 255, 0.50);
    padding: 15px;
    position: fixed;
    width: 100%;
    z-index: 100;
    transition: .3s;
    &.color{
        background: black;
    }
    &__content{
        display: flex;
        justify-content: space-between;
    }
}
</style>