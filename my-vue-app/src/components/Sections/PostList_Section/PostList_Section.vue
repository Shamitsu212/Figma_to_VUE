<script setup>
    import Post from '../../UI/Post/Post.vue';
    import post1 from '../../../assets/images/post/1.png'
    import post2 from '../../../assets/images/post/2.png'
    import post3 from '../../../assets/images/post/3.png'
    import post4 from '../../../assets/images/post/4.png'
    import post5 from '../../../assets/images/post/5.png'
    import post6 from '../../../assets/images/post/6.png'
    import post7 from '../../../assets/images/post/7.png'

    import arrow from "../../../assets/images/arrow.png"

    const posts = [
        {id: 1, label: "Travel spots in Iceland", text: "Delectus sint nisi ut recusandae molestiae. Qui iure accusantium esse temporibus et. Aut atque vel labore officiis a dolor et. Molestiae dolor quo eius. Perferendis error eveniet sit quia occaecati excepturi nisi prod.", date: "November 24, 2021", src: post1},
        {id: 2, label:"Climbing as exercise", text:"Consequuntur voluptas quis dicta expedita in minus velit impedit deserunt. Quasi sit similique nemo praesentium excepturi commodi suscipit placeat. Incidunt libero necessitatibus. Commodi modi placeat. Sit et delenit.", date:"November 24, 2021", src: post2},
        {id: 3, label:"Meditation apps I use", text:"Sit quis quaerat expedita aut sed error facilis odit similique. Saepe culpa aut fuga aut esse quaerat. Vero vero facere perferendis d", date:"November 24, 2021", src: ''},
        {id: 4, label:"How much stuff do you actually need?", text:"Veritatis perspiciatis est dolores adipisci ut sed. Culpa eligendi sunt cupiditate aut est. Recusandae pariatur qui quo animi exercitationem sint voluptas tenetur ut. Nihil", date:"November 24, 2021", src: ''},
        {id: 5, label:"The move to mirrorless cameras", text:"Maxime quisquam non in et iusto voluptates. Minima et deleniti laboriosam. Qui deleniti quas ex expedita hic facere commodi esse veniam.", date:"November 24, 2021", src: post3},
        {id: 6, label:"Drone photography on a space budget", text:"Aut quia voluptatem rem assumenda dolorem eos nostrum. Voluptatem facere ipsum aut maxime ab. Ea et voluptatum maiores odit voluptatib", date:"November 24, 2021", src: post4},
        {id: 7, label:"How to make the perfect cup of coffee", text:"Aut nihil suscipit voluptas libero deleniti similique maxime. Ea rerum illo assumenda delectus ipsum dolores nam. Reiciendis", date:"November 24, 2021", src: post5},
        {id: 8, label:"Decision fatigue & minimalism", text:"Accusamus nihil qui iste consequatur iste labore maiores nobis natus. Maiores harum accusantium. Hic sunt aut vel et hic. Et quas necessitatibus. Iusto est sit. Rerum id ut. Id dolore voluptatem eum perferendis vitae.", date:"November 24, 2021", src: ''},
        {id: 9, label:"Minimal interior design", text:"Aliquam quae nemo amet quia quae perferendis earum. Labore molestiae quis doloremque. At perferendis pariatur minima rerum delectus. Hic cum eum voluptas.", date:"November 24, 2021", src: ''},
        {id: 10, label:"The best pen I've ever used", text:"Mollitia voluptatum cum consequatur possimus ut veritatis quod non sint. Voluptatibus fuga ut magnam culpa quasi. Odio commodi modi vero dolore. Esse aut et distinctio. Voluptatem corrupti quasi. Ut omnis reprehenderi", date:"November 24, 2021", src: post6},
        {id: 11, label:"EDC must-haves", text:"Nisi ad perferendis quia modi a. Magni ut aut voluptatum. Dolorem vero molestiae itaque. Qui itaque itaque. Nihil autem perspiciatis sed similique dolor excepturi harum. Perspiciatis suscipit unde aliq", date:"November 24, 2021", src: ''},
        {id: 12, label:"Journals & how to use them", text:"Assumenda aut eos et consequatur sint vitae fugit. Nulla voluptatibus et voluptatum sed.", date:"November 24, 2021", src: ''},
        {id: 13, label:"Minimalism in the workplace?", text:"Nostrum quia sapiente natus consequatur. Dicta debitis aut minus consectetur est officiis aut. Atque itaque quia asperiores odit in tempore nisi qui. Sit ut aut ipsa v", date:"November 24, 2021", src: ''},
        {id: 14, label:"How I structure my work", text:"Inventore alias consequatur accusantium ut explicabo aut. Et fuga voluptatem est reiciendis officia qui qui. Dolorem est sequi numquam ratione cum sequi porro. Sint debitis delectus nihil placeat dolor non laborum iusto", date:"November 24, 2021", src: ''},
        {id: 15, label:"Tech-focused travel backpack", text:"Delectus et iusto perspiciatis impedit dolor eligendi sit. Voluptatem excepturi temporibus fugit molestiae. Nesciunt sequi molestiae. Molestiae recusandae sed esse illo nobis. Qui aut porro id. Tempore sed", date:"November 24, 2021", src: post7},
    ]

    
</script>

<template>
    <section class="Section">

        <Post 
            v-for="post in posts"
            :key="post.id"
            :post="post"
        />

        <a class="Section__a">
            View archive <img :src="arrow" class="a__arrow">
        </a>

    </section>
</template>

<style scoped>
    .Section{
        width: 1440px;
        height: 2536px;
        
        background-color: #FAFAFA;

        padding-top: 122px;

        display: flex;
        flex-direction: column;
        align-items: center;
    }
    .Section__a{
        margin-top: 60px;

        display: flex;
        flex-direction: row;
        align-items: center;
        gap: 3px;

        color: #575445;
        font-size: 15px;
        line-height: 22.4px;
        letter-spacing: 0;
        font-weight: 400;
        font-style: Regular;
    }
    .a__arrow{
        width: 18px;
        height: 15px;
    }
</style>