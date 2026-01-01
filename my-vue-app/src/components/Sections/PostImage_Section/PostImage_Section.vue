<script setup>
    import BigPostImage from '../../UI/PostImages/BigPostImage.vue';
    import post1 from "../../../assets/images/post/1.png"
    import MediumPostImage from '../../UI/PostImages/MediumPostImage.vue';
    import post4 from "../../../assets/images/post/4.png"
    import post5 from "../../../assets/images/post/5.png"
    import SmallPostImage from '../../UI/PostImages/SmallPostImage.vue';
    import post2 from "../../../assets/images/post/2.png"
    import post3 from "../../../assets/images/post/3.png"
    import post6 from "../../../assets/images/post/6.png"
    import post7 from "../../../assets/images/post/7.png"
    import post8 from "../../../assets/images/post/8.png"
</script>

<template>
    <div class="Section">

        <div class="Section__Container1">
            
            <BigPostImage 
                theme="TRAVEL" 
                title="Travel spots in Iceland" 
                text="Delectus sint nisi ut recusandae molestiae. Qui iure accusantium esse temporibus et. Aut atque vel labore officiis a dolor et. Molestiae dolor quo eius. Perferendis error eveniet sit quia occaecati excepturi nisi prod." 
                date="November 24, 2021"
                :src="post1"
            />

            <div class="Container1__Collumn">
                <SmallPostImage 
                    theme="EXERCISE"
                    title="Climbing as exercise"
                    date="November 24, 2021"
                    :src="post2"
                />
                <SmallPostImage 
                    theme="TECH"
                    title="The move to mirrorless cameras"
                    date="November 24, 2021"
                    :src="post3"
                />
            </div>

        </div>

        <div class="Section__Container2">
            <MediumPostImage 
                theme="TECH" 
                title="Drone photography on a space budget" 
                date="November 24, 2021" 
                :src="post4" 
            />
            <MediumPostImage 
                theme="TUTORIAL" 
                title="How to make the perfect cup of coffee"
                date="November 24, 2021" 
                :src="post5"
            />
        </div>

        <div class="Section__Container3">
            <SmallPostImage 
                theme="REVIEW"
                title="The best pen I've ever used"
                date="November 24, 2021"
                :src="post6"
            />
            <SmallPostImage 
                theme="REVIEW"
                title="Tech-focused travel backpack"
                date="November 24, 2021"
                :src="post7"
            />
            <SmallPostImage 
                theme="REVIEW"
                title="Desk accessories to keep you organized"
                date="November 24, 2021"
                :src="post8"
            />
        </div>
        
    </div>
</template>

<style scoped>
    .Section{
        width: 1440px;
        height: 1392px;

        display: flex;
        flex-direction: column;
        align-items: center;

        background-color: #FAFAFA;
    }
    .Section__Container1{
        width: 768px;
        height: 553px;

        margin-top: 105px;

        display: flex;
        flex-direction: row;
        gap: 16px;
    }
    .Container1__Collumn{
        width: 245px;
        height: 553px;

        display: flex;
        flex-direction: column;
        gap: 16px;
    }
    .Section__Container2{
        width: 768px;
        height: 334px;

        margin-top: 16px;

        display: flex;
        flex-direction: row;
        gap: 16px;
    }
    .Section__Container3{
        width: 768px;
        height: 273px;

        margin-top: 16px;

        display: flex;
        flex-direction: row;
        gap: 16px;
    }
</style>
