<template>
  <footer id="footer">
    <div class="footer__content container">  
        <ContactMeTitle />
        <div class="footer__content-socials">
            <ContactMeSocials />
        </div>
        <div class="footer__content-info">
            <ContactMePersonal />   
        </div>
    </div>
  </footer>
</template>

<script setup>
import ContactMeTitle from "./ContactMeTitle.vue";
import ContactMeSocials from "./ContactMeSocials.vue";
import ContactMePersonal from "./ContactMePersonal.vue";

</script>

<style lang="scss">

#footer{
    background: rgba(8, 0, 17, 0.9);
}

.footer__content{
    display: flex;
    justify-content: space-between;
    align-items: center;
}

.footer__content-socials-item img{
   width: 35px;
   height: 35px;
}

.footer__content-info{
    display: flex;
    gap: 10px;
}

</style>