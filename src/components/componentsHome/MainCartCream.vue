

<script setup lang="ts">
let items = [{
    img: 1,
    title: 'Creamy Chocolate Cake',
    price: '$140',
}, {
    img: 5,
    title: 'Vanilla Ice Cream',
    price: '$120',
}, {
    img: 3,
    title: 'Strawberry Shortcake ',
    price: '$150',
}, {
    img: 4,
    title: 'Blueberry Cheesecake ',
    price: '$160',
}, {
    img: 5,
    title: 'Creamy White Forest',
    price: '$180',
}, {
    img: 6,
    title: 'Fruit Cherry Cake',
    price: '$180',
}, {
    img: 3,
    title: 'Muffets Burger Bun',
    price: '$180',
}, {
    img: 2,
    title: 'Creamy Chocolate Cake ',
    price: '$180',
},
{
    img: 2,
    title: 'Creamy Chocolate Cake ',
    price: '$180',
}];

        // thay các giá trị trong mảng này để lặp lại với các giá trị khác nhau cho img, h6 và span
        
    

</script>

<template>
        <div v-for="(item, index) in items" :key="index" class="cart-cream ">
            <div class="img-cream">
                <img :src="`/assets/img/main.cream/${item.img}.jpg`" alt="">
            </div>
            <div class="cart-cream-title">
                <h6>
                    {{ item.title }}
                </h6>
                <div class="price">
                    <span>
                        {{ item.price }}
                    </span>
                </div>
            </div>
        </div>
</template>

<style scoped></style>
