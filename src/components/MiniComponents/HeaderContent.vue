<template>
    <header class="header">
        <div class="header__content container">
            <HeaderContentTitle />
        </div>
    </header>
</template>

<script setup>
import HeaderContentTitle from "../MiniComponents/HeaderContentTitle.vue";
</script>

<style lang="scss">

.header{
    display: flex;
    background: url('../../assets/images/header-bg.png');
    background-size: cover;
    background-position: center;
    height: 850px;
    width: 100%;
    position: relative;
    &::before{
        content: '';
        width: 100%;
        height: 100%;
        background:rgba(0,0,0,.5);
        position: absolute;
        border-radius: 6px;
        transition: 0.5s;
    }
}

.header__content{
    display: flex;
    justify-content: center;
    align-items: center;
    text-align: center;
}

</style>