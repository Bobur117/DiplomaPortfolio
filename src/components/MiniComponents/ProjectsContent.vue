<template>
    <seciton id="projects">
        <ProjectsContentTitle />
        
        <div class="projects__content">
            <div class="projetcs__content-items">
                <ProjectContentItem />
            </div>
        </div>
    </seciton>
  
</template>

<script setup>
import ProjectContentItem from "./ProjectContentItem.vue";
import ProjectsContentTitle from "./ProjectsContentTitle.vue";

</script>

<style lang="scss">

.projetcs__content-items{
    display: flex;
    justify-content: center;
    align-items: center;
}

</style>