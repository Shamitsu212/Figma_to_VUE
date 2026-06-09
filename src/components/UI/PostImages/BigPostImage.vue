<script setup>

    const props = defineProps({
        
        theme:{
            type: String,
            default: 'Travel' 
        },
        title:{
            type: String,
            default: 'Title..' 
        },
        text: {
            type: String,
            default: 'text..' 
        },
        date: {
            type: String,
            default: 'Month date year' 
        },
        src: {
            type: String,
            required: true
        }
    })
</script>

<template>
    <article class="Post">

        <div class="Post__wrapper">
            <img :src="src" class="wrapper__img"/>
        </div>

        <div class="Post__Content">
            <div class="Content__Theme">
                {{ theme }}
            </div>
            <h2 class="Content__Title">
                {{ title }}
            </h2>
            <p class="Content__Text">
                {{ text }}
            </p>
            <time class="Content__Date">
                {{ date }}
            </time>
        </div>

    </article>
</template>

<style scoped>
    .Post{
        width: 507px;
        height: 553px;

        display: flex;
        flex-direction: column;

        background-color: white;
    }
    .Post__wrapper{
        width: 505px;
        height: 284px;
    }
    .wrapper__img{
        width: 100%;
        height: 100%;
    }
    .Post__Content{
        width: 505px;
        height: 266px;

        display: flex;
        flex-direction: column;
        padding-left: 20px;
    }
    .Content__Theme{
        width: 59px;
        height: 12px;

        color: #353732;
        font-size: 12px;
        line-height: 12px;
        letter-spacing: 2px;
        font-weight: 400;
        font-style: Regular;

        margin-top: 20px;
    }
    .Content__Title{
        width: 255px;
        height: 34px;

        color: #45525B;
        font-size: 25px;
        line-height: 33.6px;
        letter-spacing: 0;
        font-weight: 400;
        font-style: Regular;

        margin-top: 9px;
    }
    .Content__Text{
        width: 465px;
        height: 66px;

        color: #45525B;
        font-size: 14px;
        line-height: 22.4px;
        letter-spacing: 0;
        font-weight: 400;
        font-style: Regular;

        margin-top: 12px;
    }
    .Content__Date{
        width: 96px;
        height: 17px;

        color: #45525B;
        font-size: 11px;
        line-height: 26.8px;
        letter-spacing: 0;
        font-weight: 400;
        font-style: Regular;

        margin-top: 59px;
    }
</style>
