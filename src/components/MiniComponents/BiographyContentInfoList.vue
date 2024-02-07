<template>
    <tr class="biography__content-info-descr">
        <th>
            {{ text.title }}:
        </th>
        <td>
            {{ text.value }}
        </td>
    </tr>
  
</template>

<script setup>
const props = defineProps(['text']);

</script>

<style lang="scss">

.biography__content-info-descr{
    font-family: 'Montserrat';
    font-size: 24px;
    color: white;
}

td, th {
    padding: 7px;
    vertical-align: top;
    text-align: left;
}

td{
    font-style: italic;
}
</style>