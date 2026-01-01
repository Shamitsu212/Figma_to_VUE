<script setup>
    import Button_UI from '../../UI/Button_UI.vue';
    import Input_UI from '../../UI/Input_UI.vue';

    import { ref } from 'vue';

    const name = ref('')
    const email = ref('')

</script>

<template>
    <div class="Section">
        
        <div class="Section__Text">
            <h3 class="Text__Title">
                Stay in the know.
            </h3>    
            <p class="Text_p">
                <span class="p__span">Sign-up to my newsletter to get an update whenever</span> 
                <span class="p__span">I post a new article. I try to be very mindful of not</span>
                <span class="p__span">spamming my subscribers.</span>
            </p>
        </div>

        <form class="Section__Form">
            <Input_UI type="text" label="Name" placeholder="" v-model="name"/>
            <Input_UI type="email" label="Email Address" placeholder="" v-model="email"/>
            <Button_UI text=""/>
        </form>

    </div>
</template>

<style scoped>

    .Section{
        width: 1440px;
        height: 387px;

        display: flex;
        flex-direction: row;
        gap: 16;

        padding-left: 336px;
        padding-top: 102px;

        background-color: white;
    }

    .Section__Text{
        width: 376px;
        height: 187px;

        display: flex;
        flex-direction: column;
        gap: 11px;
    }

    .Text__Title{
        width: 222px;
        height: 39px;

        margin-top: 20px;

        color: #353732;
        font-size: 28px;
        line-height: 38.4px;
        font-style: Regular;
        letter-spacing: 0;
        font-weight: 400;
    }

    .Text_p{
        display: flex;
        flex-direction: column;
    }

    .p__span{
        color: #353732;
        font-size: 16px;
        line-height: 22.4px;
        font-style: Regular;
        letter-spacing: 0;
        font-weight: 400;
    }
    .Section__Form{
        width: 376.6px;
        height: 171.82px;

        display: flex;
        flex-direction: column;
        gap: 10px;
    }

</style>