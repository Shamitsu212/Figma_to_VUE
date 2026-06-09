<script setup>
    import MediumLogo from '../../UI/Logo/MediumLogo.vue'; 
</script>

<template>
    
    <footer class="footer">

        <div class="footer_Content">
            <div class="Content__Logo">
                <MediumLogo />
            </div>
            <p class="Content__p">
                A lifestyle blog about minimalism, technology, design & travel. Powered by Webflow.
            </p>

            <nav class="Content__nav">

                <div class="nav__Row">
                    <a class="nav__a">
                        Start
                    </a>
                    <a class="nav__a">
                        Archive
                    </a>
                </div>

                <div class="nav__Row">
                    <a class="nav__a">
                        Instructions
                    </a>
                    <a class="nav__a">
                        Style guide
                    </a>
                    <a class="nav__a">
                        Licenses
                    </a>
                    <a class="nav__a">
                        Changelog
                    </a>
                </div>

            </nav>
        </div>

    </footer>

</template>

<style scoped>
    .footer{
        width: 1440px;
        height: 356px;
        
        background-color: white;

        display: flex;
        flex-direction: column;
        align-items: center;
        justify-content: center;
    }
    .footer_Content{
       width: 800px;
       height: 156px;
       
       display: flex;
       flex-direction: column;
    }
    .Content__Logo{
        width: 78px;
        height: 40px;
    }
    .Content__p{
        width: 600px;
        height: 23px;

        margin-top: 20px;

        color: #353732;
    }
    .Content__nav{
        display: flex;
        flex-direction: column;
    }
    .nav__Row{
        display: flex;
        flex-direction: row;
        gap: 20px;

        margin-top: 19px;
    }
    .nav__a{
        color: #45525B;
        font-size: 14px;
        line-height: 22.4px;
        font-weight: 400;
        font-style: Regular;
    }
</style>