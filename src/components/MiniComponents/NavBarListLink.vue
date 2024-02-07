<template>
    <li>
        <a :href="'#' + link.section" class="nav__content-list-link">
            {{ link.title }}
        </a>
    </li>
</template>

<script setup>

const props = defineProps(['link']); 

</script>

<style lang="scss">
.nav__content-list-link{
    font-family: 'Montserrat';
    font-size: 20px;
    color: white;
}
</style>