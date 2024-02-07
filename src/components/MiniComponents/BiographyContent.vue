<template>
    <seciton id="biography">
        <h1 class="biography-title">
            Biography
        </h1> 
        <div class="biography__content">
            <BiographyContentImg />
            <BiographyContentInfo />
        </div>
        
    </seciton>
</template>

<script setup>
import BiographyContentImg from "./BiographyContentImg.vue";
import BiographyContentInfo from "./BiographyContentInfo.vue";

</script>

<style lang="scss">

#biography{
    margin-top: 50px;
}

.biography-title{
    font-family: 'Montserrat';
    font-size: 32px;
    color: white;
    text-align: center;
    padding-top: 10px; 
    padding-bottom: 10px;
    border-bottom: 3px solid rgba(255, 255, 255, .5);
    border-top:  3px solid rgba(255, 255, 255, .5);
    margin-bottom: 50px;
}

.biography__content{
    display: flex;
    gap: 35px;
    margin-bottom: 50px;
}


</style>