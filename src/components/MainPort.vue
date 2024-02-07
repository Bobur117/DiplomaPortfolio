<template>
    <main class="main">
        <div class="main__content container">
            <BiographyContent />
            <ProjectsContent />
        </div>
    </main>
  
</template>

<script setup>
import BiographyContent from "./MiniComponents/BiographyContent.vue";
import ProjectsContent from "./MiniComponents/ProjectsContent.vue";

</script>

<style lang="scss">
.main{
    background:rgba(1, 14, 48, 0.9);
    padding-top: 50px;
}

</style>