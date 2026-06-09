<script setup>
    import MediumLogo from '../../UI/Logo/MediumLogo.vue';
</script>

<template>
    <section class="Section">

        <div class="Section__Content">
            <div class="Content__Logo">
                <MediumLogo />
            </div>

            <h1 class="Content__H">
                <span class="H__Text">Welcome to Calm – a lifestyle blog about</span>
                <span class="H__Text">minimalism, technology, design & travel.</span>
            </h1>
        </div>
        
       
    </section>
</template>

<style scoped>
    .Section{
        background-color: white;

        width: 1440px;
        height: 438px;

        display: flex;
        flex-direction: column;
        align-items: center;
        justify-content: center;
    }
    .Section__Content{
        width: 800px;
        height: 148px;
        
        display: flex;
        flex-direction: column;
        justify-content: center;
        gap: 17px;
    }

    .Content__Logo{
        width: 94px;
        height: 48px;
    }
    .Content__H{
        width: 683px;
        height: 80px;

        display: flex;
        flex-direction: column;
    }
    .H__Text{
        font-weight: 400;
        font-style: Regular;
        font-size: 36px;
        line-height: 40px;
        letter-spacing: 0;
        color: #353732;
    }
</style>