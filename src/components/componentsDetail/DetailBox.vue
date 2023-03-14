

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
}];
 // thay các giá trị trong mảng này để lặp lại với các giá trị khác nhau cho img, h6 và span

</script>

<template>
    <div class="box"  v-for="(item, index) in items" :key="index">
        <img :src="`/assets/img/main.time/${item.img}.png`" alt="">
        <div class="product-option">
            <i class="fa-regular fa-eye"></i>
            <i class="fa-solid fa-code-compare"></i>
            <i class="fa-regular fa-heart"></i>
        </div>
        <div class="content">
            <span style="font-weight:800;
                
                                                                            height: 20px;
                                                                            font-size: 14px;">Muffets & Tuffets Whole
            </span>
            <span style="font-weight: 800;
                                                                            height: 20px;
                                                                            font-size: 14px;">Wheat Bread 400 g</span>
            <div class="price">
                <span style="font-weight: 600;margin-top: 10px;;color: #d99f46;">$26.69</span>
                <span style="font-weight: 400;
                                                                            margin-left: 6px;
                                                                            font-size: calc(13px + (14 - 13) * ((100vw - 320px) / (1920 - 320)));    text-decoration: line-through;
                                                                            color: #4a5568;">28.56</span>
            </div>

          

            <button class="add">Add
                <i class="fa-solid fa-plus"></i>

            </button>
        </div>
    </div>
</template>

<style scoped>
               /* <div class="box">
                    <img src="/assets/img/main.time/1.png" alt="">
                    <div class="product-option">
                        <i class="fa-regular fa-eye"></i>
                        <i class="fa-solid fa-code-compare"></i>
                        <i class="fa-regular fa-heart"></i>
                    </div>
                    <div class="content">
                        <span style="font-weight:800;
                
                                                                        height: 20px;
                                                                        font-size: 14px;">Muffets & Tuffets Whole
                        </span>
                        <span style="font-weight: 800;
                                                                        height: 20px;
                                                                        font-size: 14px;">Wheat Bread 400 g</span>
                        <div class="price">
                            <span style="font-weight: 600;margin-top: 10px;;color: #d99f46;">$26.69</span>
                            <span style="font-weight: 400;
                                                                        margin-left: 6px;
                                                                        font-size: calc(13px + (14 - 13) * ((100vw - 320px) / (1920 - 320)));    text-decoration: line-through;
                                                                        color: #4a5568;">28.56</span>
                        </div>

                        <div class="check" style="margin-top: 10px;font-size: 12px;">
                            <span class="fa fa-star checked"></span>
                            <span class="fa fa-star checked"></span>
                            <span class="fa fa-star checked"></span>
                            <span class="fa fa-star checked"></span>
                            <span class="fa fa-star"></span>
                        </div>

                        <button class="add">Add
                            <i class="fa-solid fa-plus"></i>

                        </button>
                    </div>
                </div>
                <div class="box">
                    <img src="/assets/img/main.time/3.png" alt="">
                    <div class="product-option">
                        <i class="fa-regular fa-eye"></i>
                        <i class="fa-solid fa-code-compare"></i>
                        <i class="fa-regular fa-heart"></i>
                    </div>
                    <div class="content">
                        <span style="font-weight:800;
                
                                                                        height: 20px;
                                                                        font-size: 14px;">Muffets & Tuffets Whole
                        </span>
                        <span style="font-weight: 800;
                                                                        height: 20px;
                                                                        font-size: 14px;">Wheat Bread 400 g</span>
                        <div class="price">
                            <span style="font-weight: 600;margin-top: 10px;;color: #d99f46;">$26.69</span>
                            <span style="font-weight: 400;
                                                                        margin-left: 6px;
                                                                        font-size: calc(13px + (14 - 13) * ((100vw - 320px) / (1920 - 320)));    text-decoration: line-through;
                                                                        color: #4a5568;">28.56</span>
                        </div>

                        <div class="check" style="margin-top: 10px;font-size: 12px;">
                            <span class="fa fa-star checked"></span>
                            <span class="fa fa-star checked"></span>
                            <span class="fa fa-star checked"></span>
                            <span class="fa fa-star checked"></span>
                            <span class="fa fa-star"></span>
                        </div>

                        <button class="add">Add
                            <i class="fa-solid fa-plus"></i>

                        </button>
                    </div>
                </div>
                <div class="box">
                    <img src="/assets/img/main.time/4.png" alt="">
                    <div class="product-option">
                        <i class="fa-regular fa-eye"></i>
                        <i class="fa-solid fa-code-compare"></i>
                        <i class="fa-regular fa-heart"></i>
                    </div>
                    <div class="content">
                        <span style="font-weight:800;
                
                                                                        height: 20px;
                                                                        font-size: 14px;">Muffets & Tuffets Whole
                        </span>
                        <span style="font-weight: 800;
                                                                        height: 20px;
                                                                        font-size: 14px;">Wheat Bread 400 g</span>
                        <div class="price">
                            <span style="font-weight: 600;margin-top: 10px;;color: #d99f46;">$26.69</span>
                            <span style="font-weight: 400;
                                                                        margin-left: 6px;
                                                                        font-size: calc(13px + (14 - 13) * ((100vw - 320px) / (1920 - 320)));    text-decoration: line-through;
                                                                        color: #4a5568;">28.56</span>
                        </div>

                        <div class="check" style="margin-top: 10px;font-size: 12px;">
                            <span class="fa fa-star checked"></span>
                            <span class="fa fa-star checked"></span>
                            <span class="fa fa-star checked"></span>
                            <span class="fa fa-star checked"></span>
                            <span class="fa fa-star"></span>
                        </div>

                        <button class="add">Add
                            <i class="fa-solid fa-plus"></i>

                        </button>
                    </div>
                </div>
                <div class="box">
                    <img src="/assets/img/main.time/5.png" alt="">
                    <div class="product-option">
                        <i class="fa-regular fa-eye"></i>
                        <i class="fa-solid fa-code-compare"></i>
                        <i class="fa-regular fa-heart"></i>
                    </div>
                    <div class="content">
                        <span style="font-weight:800;
                
                                                                        height: 20px;
                                                                        font-size: 14px;">Muffets & Tuffets Whole
                        </span>
                        <span style="font-weight: 800;
                                                                        height: 20px;
                                                                        font-size: 14px;">Wheat Bread 400 g</span>
                        <div class="price">
                            <span style="font-weight: 600;margin-top: 10px;;color: #d99f46;">$26.69</span>
                            <span style="font-weight: 400;
                                                                        margin-left: 6px;
                                                                        font-size: calc(13px + (14 - 13) * ((100vw - 320px) / (1920 - 320)));    text-decoration: line-through;
                                                                        color: #4a5568;">28.56</span>
                        </div>

                        <div class="check" style="margin-top: 10px;font-size: 12px;">
                            <span class="fa fa-star checked"></span>
                            <span class="fa fa-star checked"></span>
                            <span class="fa fa-star checked"></span>
                            <span class="fa fa-star checked"></span>
                            <span class="fa fa-star"></span>
                        </div>

                        <button class="add">Add
                            <i class="fa-solid fa-plus"></i>

                        </button>
                    </div>
                </div>
                <div class="box">
                    <img src="/assets/img/main.time/6.png" alt="">
                    <div class="product-option">
                        <i class="fa-regular fa-eye"></i>
                        <i class="fa-solid fa-code-compare"></i>
                        <i class="fa-regular fa-heart"></i>
                    </div>
                    <div class="content">
                        <span style="font-weight:800;
                
                                                                        height: 20px;
                                                                        font-size: 14px;">Muffets & Tuffets Whole
                        </span>
                        <span style="font-weight: 800;
                                                                        height: 20px;
                                                                        font-size: 14px;">Wheat Bread 400 g</span>
                        <div class="price">
                            <span style="font-weight: 600;margin-top: 10px;;color: #d99f46;">$26.69</span>
                            <span style="font-weight: 400;
                                                                        margin-left: 6px;
                                                                        font-size: calc(13px + (14 - 13) * ((100vw - 320px) / (1920 - 320)));    text-decoration: line-through;
                                                                        color: #4a5568;">28.56</span>
                        </div>

                        <div class="check" style="margin-top: 10px;font-size: 12px;">
                            <span class="fa fa-star checked"></span>
                            <span class="fa fa-star checked"></span>
                            <span class="fa fa-star checked"></span>
                            <span class="fa fa-star checked"></span>
                            <span class="fa fa-star"></span>
                        </div>

                        <button class="add">Add
                            <i class="fa-solid fa-plus"></i>

                        </button>
                    </div>
                </div> */
</style>
