<script setup> 

    const props = defineProps({
        post: {
            type: Object,
            required: true
        }
    })

</script>

<template>
    <article class="post">
        <div class="post__wrapper" v-if="post.src.length != 0">
            <img :src="post.src" class="wrapper__img">
        </div>
        <div class="post_Content">
            <h4 class="Content__H">
                {{ post.label }}
            </h4>

            <p class="Content__P">
                {{ post.text }}
            </p>

            <date class="Content__Date">
                {{ post.date }}
            </date>
        </div>

    </article>
</template>

<style scoped>
    .post{
        width: 767px;
        min-height: 150px;
        max-height: 175px;

        padding-top: 20px;

        display: flex;
        flex-direction: row;
        gap: 20px;
    }
    .post__wrapper{
        min-width: 200px;
        height: 122px;

        border-radius: 10px;
        overflow: hidden;
    }
    .wrapper__img{
        width: 100%;
        height: 100%;
    }
    .post_Content{
        min-width: 538px;
        max-width: 767px;
        min-height: 68px;
        max-height: 150px;

        display: flex;
        flex-direction: column;
    }
    .Content__H{
        min-width: 173px;
        height: 24px;

        color: #45525B;
        font-size: 17px;
        line-height: 24px;
        letter-spacing: 0;
        font-weight: 400;
        font-style: Regular;
    }
    .Content__P{
        min-width: 530px;
        max-width: 753px;
        min-height: 45px;
        max-height: 68px;

        color: #45525B;
        font-size: 16px;
        line-height: 22.4px;
        letter-spacing: 0;
        font-weight: 400;
        font-style: Regular;

        margin-top: 2px;
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

        margin-top: 6px;
    }
</style>