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
            <time class="Content__Date">
                {{ date }}
            </time>
        </div>

    </article>
</template>

<style scoped>
    .Post{
        width: 243.31px;
        height: 270.84px;

        display: flex;
        flex-direction: column;

        background-color: white;
    }
    .Post__wrapper{
        width: 243px;
        height: 137px;
    }
    .wrapper__img{
        width: 100%;
        height: 100%;
    }
    .Post__Content{
        width: 243px;
        height: 143.75px;

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

        margin-top: 17px;
    }
    .Content__Title{
        min-width: 196px;
        height: 22px;

        color: #45525B;
        font-size: 16px;
        line-height: 21.6px;
        letter-spacing: 0;
        font-weight: 400;
        font-style: Regular;

        margin-top: 3px;
    }
    .Content__Date{
        width: 96px;
        height: 17px;

        color: #45525B;
        font-size: 11px;
        line-height: 16.8px;
        letter-spacing: 0;
        font-weight: 400;
        font-style: Regular;

        margin-top: 30px;
    }
</style>
