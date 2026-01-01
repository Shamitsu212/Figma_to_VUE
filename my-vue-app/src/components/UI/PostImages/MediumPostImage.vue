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
        width: 374px;
        height: 332px;

        display: flex;
        flex-direction: column;

        background-color: white;
    }
    .Post__wrapper{
        width: 374px;
        height: 210px;
    }
    .wrapper__img{
        width: 100%;
        height: 100%;
    }
    .Post__Content{
        width: 374px;
        height: 121px;

        display: flex;
        flex-direction: column;
        padding-left: 20px;
    }
    .Content__Theme{
        width: 42px;
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
        min-width: 304px;
        height: 24px;

        color: #45525B;
        font-size: 17px;
        line-height: 24px;
        letter-spacing: 0;
        font-weight: 400;
        font-style: Regular;

        margin-top: 10px;
    }
    .Content__Date{
        min-width: 98px;
        height: 17px;

        color: #45525B;
        font-size: 11px;
        line-height: 26.8px;
        letter-spacing: 0;
        font-weight: 400;
        font-style: Regular;

        margin-top: 10px;
    }
</style>
