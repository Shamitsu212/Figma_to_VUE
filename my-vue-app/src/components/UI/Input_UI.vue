<script setup> 

    const props = defineProps({
        type:{
            type: String,
            default: "Поле ввода"
        },
        label:{
            type: String,
            default: "Поле ввода"
        },
        placeholder:{
            type: String,
            default: "Ввод"
        },
        modelValue:{
            type: String,
            default: ""
        }
    })

    const emit = defineEmits(["update:modelValue"])

    function onInput(event){
        emit("update:modelValue", event.target.value)
    }
</script>

<template>

    <div class="Container">

        <label class="Container__Label">
            {{ label}}
        </label>

        <input 
            :type="type" 
            :value="modelValue" 
            :placeholder="placeholder"
            @input="onInput" 
            
            class="Container__Input"
        />

    </div>

</template>

<style scoped>

    .Container{
        width: 376px;
        height: 57px;

        display: flex;
        flex-direction: column;
        gap: 0;
    }

    .Container__Label{
        min-width: 33px;
        height: 20px;

        color: #353732;
        font-size: 12px;
        line-height: 19.6px;
        font-weight: 400;
        font-style: Regular;
    }
    .Container__Input{
        width: 376px;
        height: 38px;

        border-radius: 8px;
        border: 1px solid #E5E7EB;

        color: #52503B05;
    }
</style>