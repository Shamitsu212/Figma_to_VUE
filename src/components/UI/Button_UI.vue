<script setup> 

    const props = defineProps({
        text:{
            type: String,
        }
    })
    
</script>

<template>
    <button class="button">
        {{ text }}
    </button>
</template>

<style scoped>
    .button{
        width: 82px;
        height: 32px;

        border: none;
        border-radius: 6px;

        background-color: #353732;
        color: white;
    }
</style>