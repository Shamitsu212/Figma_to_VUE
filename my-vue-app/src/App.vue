<script setup>
    import Header from "./components/Layout/Header/Header.vue"
import InputSection from "./components/Sections/Input_Section/InputSection.vue";
    import PostImage_Section from "./components/Sections/PostImage_Section/PostImage_Section.vue";
    import Welcome_Section from "./components/Sections/Welcome_Section/Welcome_Section.vue";
</script>

<template>
    <div class="app">
        <Header />
        <Welcome_Section/>
        <PostImage_Section />
        <InputSection />
    </div>
</template>

<style scoped>
    .app{
        width: 100%;

        display: flex;
        flex-direction: column;
        align-items: center;

        background-color: black;
    }
</style>
