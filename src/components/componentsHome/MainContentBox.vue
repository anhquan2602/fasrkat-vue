

<script setup lang="ts">

let items = [{
    img: 1,
    title: 'Muffets & Tuffets Whole Wheat Bread 400 g',
    price: '$140',
}, {
    img: 8,
    title: 'Peanut Butter Bite Premium Butter Cookies 600 g',
    price: '$120',
}, {
    img: 3,
    title: 'Yumitos Chilli Sprinkled Potato Chips 100 ',
    price: '$150',
}, {
    img: 4,
    title: 'Fresh Bread and Pastry Flour 200 ',
    price: '$160',
}, {
    img: 5,
    title: 'Fresh Bread and Pastry Flour 200 g',
    price: '$180',
}, {
    img: 6,
    title: 'SnackAmor Combo Pack of Jowar Stick and Jowar Chip',
    price: '$180',
}, {
    img: 7,
    title: 'Fantasy Crunchy Choco Chip Cookies',
    price: '$180',
}, {
    img: 2,
    title: 'Milky Silicone Heart Chocolate Mould ( Pack of 1 )',
    price: '$180',
}];
 // thay các giá trị trong mảng này để lặp lại với các giá trị khác nhau cho img, h6 và span


</script>


<template>
    <div v-for="(item, index) in items" :key="index" class="box">

        <img :src="`/assets/img/main.time/${item.img}.png`" alt="">
        <div class="product-option">


        </div>
        <div class="content">
            <h3>

                {{ item.title }}

            </h3>
            <span class="fw600 col-yel">
                {{ item.price }}

            </span>




            <button></button>
        </div>
    </div>
</template>

<style scoped></style>
