<template>
    <div class="biography__content-info">
        <table>
            <BiographyContentInfoList v-for="text in texts" :key="text.title" :text="text"/>
        </table>
    </div>
</template>

<script setup>
import BiographyContentInfoList from "./BiographyContentInfoList.vue";

const texts = [
    
{
    title: 'Full name',
    value: 'Boburmirzo Ibrokhimov Burhonjon Ogli'
},
{
    title: 'Date of birth',
    value: 'May 11, 1997'
},
{
    title: 'Workplace',
    value: 'Westminster International University in Tashkent'
},
{
    title: 'Degree',
    value: 'Master of Science in Applied Economics, Bachelor of Science in Economics and Finance'
},
{
    title: 'Professional goal',
    value: 'To become a senior specialist in Web programming in the very near future'
},
{
    title: 'Mission statement',
    value: 'No excellence can be acquired without constanct practice'
},
{
    title: 'Skills and expertise',
    value: 'Attention to detail, creativity, memory, mathematical skills, analytical mindset'
},

];


</script>

<style lang="scss">

.biography__content-info{
    max-width: 500px;
}

</style>