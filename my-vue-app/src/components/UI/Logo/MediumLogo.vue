<script setup>
    import Logo from "../../../assets/images/MediumLogo.png"
</script>

<template>

    <div class="LogoBody">
        <img :src="Logo" class="LogoBody__img"/>
    </div>

</template>

<style scoped>

    .LogoBody{
        width: 94px;
        height: 48px;
        
        display: flex;
        flex-direction: row;
        align-items: center;
        justify-content: center;
        
    }

    .LogoBody__img{
        width: 100%;
        height: 100%;
        object-fit: cover;
    }

</style>
