<script setup>
    import SmallLogo from '../../UI/Logo/SmallLogo.vue';
</script>

<template>
    <header class="headerBody">

        <div class="headerBody__headerContent">
            
            <div class="headerContent__Logo">
                <SmallLogo />
            </div>

            <nav class="headerContent__nav">
                <a href="#" class="nav__a" >Home</a>
                <a href="#" class="nav__a">Archive</a>
                <a href="#" class="nav__a">About</a>
            </nav>

        </div>

    </header>
</template>

<style scoped>

    .headerBody{
        width: 1440px;
        height: 80px;

        display: flex;
        flex-direction: row;
        align-items: center;
        justify-content: center;

        background-color: white;

        position: sticky;
        top: 0;
    }
    .headerBody__headerContent{
        width: 1200px;
        height: 40px;

        display: flex;
        flex-direction: row;
        align-items: center;
        gap: 870px;
    }
    .headerContent__Logo{
        width: 78px;
        height: 40px;
    }
    .headerContent__nav{
        width: 230px;
        height: 40px;

        display: flex;
        flex-direction: row;
        align-items: center;
        gap: 20px;
    }
    .nav__a{
        color: #353732;
        font-size: 16px;
        text-decoration: none;
    }
</style>
