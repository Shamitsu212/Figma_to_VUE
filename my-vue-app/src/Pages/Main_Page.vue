<script setup>
import Footer from '../components/Layout/Footer/Footer.vue';
import Header from '../components/Layout/Header/Header.vue';
import Input_Section from '../components/Sections/Input_Section/Input_Section.vue';
import PostImage_Section from '../components/Sections/PostImage_Section/PostImage_Section.vue';
import PostList_Section from '../components/Sections/PostList_Section/PostList_Section.vue';
import Welcome_Section from '../components/Sections/Welcome_Section/Welcome_Section.vue';

 

   
    
</script>

<template>
    <div class="Page">
        <Header />
        <Welcome_Section />
        <PostImage_Section />
        <Input_Section />
        <PostList_Section />
        <Footer />
    </div>
</template>

<style scoped>
    
</style>