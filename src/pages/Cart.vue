<template>
    <!-- <div class="container-category__breadcrumb"> -->
        <Breadcrumb />
    <!-- </div> -->
    <h1>CART</h1>
</template>

<script setup>

const items = [
    {
        title: 'Главная',
        disabled: false,
        href: '/',
    },
    {
        title: 'Корзина',
        disabled: true,
        href: '/cart',
    },
]

</script>